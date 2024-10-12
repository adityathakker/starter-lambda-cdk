# Welcome to your CDK TypeScript project

## Prereqs
- AWS Account: Ensure you have an AWS account with permissions to deploy Lambda functions and related resources.
- AWS CLI: Installed and configured with your AWS credentials.
- AWS CDK: Installed globally via npm.
```bash
npm install -g aws-cdk
```
- Node.js and npm: Ensure you have Node.js (v14 or later) and npm installed.
- TypeScript: Installed globally via npm.
```bash
npm install -g typescript
```

## Build and Deploy
This is a starter project for CDK development with TypeScript.

```bash
# Navigate to the lambda directory
cd lambda

# Install Lambda dependencies
npm install

# Compile Lambda TypeScript code
npx tsc

# Navigate back to the root directory
cd ..

# Install CDK dependencies
npm install

# Compile CDK TypeScript code
npm run build

# Bootstrap CDK (if not done before)
cdk bootstrap

# Synthesize CloudFormation template
cdk synth

# Deploy the stack
cdk deploy

# Test the Lambda function via AWS CLI
aws lambda invoke --function-name StarterLambdaFunction output.json
```


## Useful CDK commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `npx cdk deploy`  deploy this stack to your default AWS account/region
* `npx cdk diff`    compare deployed stack with current state
* `npx cdk synth`   emits the synthesized CloudFormation template
