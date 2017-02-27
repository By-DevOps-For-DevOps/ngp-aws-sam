# ngp-aws-sam
1. Add the `buildspec.yaml` and `samTemplate.yaml` to Github repo containing Lambda function.
2. Use `ngp-aws-sam/codepipeline.yaml` to create a new stack from AWS cloudformation console.
3. Give the GITHUB details of the lambda function as parameters.

The Stack will create a Codepipeline which will deploy the Lambda function and create an API gateway endpoint pointing towards it.
