# ngp-aws-sam

### Pre-requisites
1. An S3 Bucket in region where we need to deploy the lambda function.
2. Github access token to access the repository containing the lambda function.

### Steps to install
1. Add the `buildspec.yaml` and `samTemplate.yaml` to Github repo containing Lambda function.
2. Use `ngp-aws-sam/codepipeline.yaml` to create a new stack from AWS cloudformation console.
3. Give the GITHUB details of the lambda function as parameters.

The Stack will create a Codepipeline which will deploy the Lambda function and create an API gateway endpoint pointing towards it.
