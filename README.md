# LambdaNodeModuleLayer
Lambda Layer For Node Module

## Deploy Command
sls deploy -c slsdeploy.yml

## Add Layer Permission Command
aws lambda add-layer-version-permission --profile lambdaserverless --layer-name  LambdaNodeModuleLayer --statement-id lambdanodemodulelayer --action lambda:GetLayerVersion --principal '*' --version-number 3

## List Policy Attached To Layer
aws lambda get-layer-version-policy --profile lambdaserverless --layer-name LambdaNodeModuleLayer --version-number 3

## Remove Layer Permission Command
aws lambda remove-layer-version-permission --profile lambdaserverless --layer-name LambdaNodeModuleLayer --statement-id lambdanodemodulelayer --version-number 3