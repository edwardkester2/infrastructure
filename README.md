# ServiceNow DevOps Stuff

This is a repo for the ServiceNow DevOps Jenkins Lab CFT and supporting files.

## Installation

Install the [AWS CLI](https://aws.amazon.com/cli/) or the [AWS CloudFormation Console](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-using-console.html) to deploy this CFT. 

## Usage

```aws cloudformation create-stack --stack-name DevOpsLabServer --template-body file://sn_jenkins_cft/jenkins_cf_deployment.yaml --parameters ParameterKey=KeyName,ParameterValue=sndevops_key ParameterKey=VpcId,ParameterValue=vpc-ID ParameterKey=SubnetId,ParameterValue=subnet-ID ParameterKey=MasterAdminPassword,ParameterValue=SuperSecretPassword! ParameterKey=GitHubUsername,ParameterValue=amittell```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
