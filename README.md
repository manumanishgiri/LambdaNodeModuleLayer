# LambdaNodeModuleLayer
Lambda Layer For Node Module

## Deploy Command
sls deploy -c slsdeploy.yml

## Add Layer Permission Command
aws lambda add-layer-version-permission --profile lambdaserverless --layer-name ffmpeg --statement-id ffmpeg --action lambda:GetLayerVersion --principal '*' --version-number 1

## Remove Layer Permission Command
aws lambda remove-layer-version-permission --profile lambdaserverless --layer-name ffmpeg --statement-id ffmpeg --version-number 1