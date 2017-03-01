# ngp-aws-sam
The Stack will create a CodePipeline which will deploy the Lambda 
function and create an API gateway endpoint pointing towards it.
### Pre-requisites
1. GitHub Token with `admin:repo_hook` and `repo` scopes to access the 
repository containing the lambda function.

### Steps to install
1. Add the `buildspec.yaml` and `samTemplate.yaml` to GitHub repo 
containing Lambda function.
2. Use `ngp-aws-sam/codepipeline.yaml` to create a new stack in 
N.Virginia (us-east-1) region from [AWS CloudFormation console] (https://console.aws.amazon.com/cloudformation/home?region=us-east-1).
Note: The region where the app will be deployed can be specified with 
`region` CF parameter. 
3. Specify the GitHub details of the lambda function as parameters.
