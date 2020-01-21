# Cloudformation Template for Hands-on AWS Practice
## Create a new Cloudformation stack
`
aws cloudformation create-stack  
    --stack-name <stack name>  
    --template-body file://<path to the template file>  
    --parameters
        ParameterKey=DBUsername,ParameterValue=<db username>
        ParameterKey=DBPassword,ParameterValue=<db password>  
        ParameterKey=EC2InstanceType,ParameterValue=<instance type>   
        ParameterKey=KeyName,ParameterValue=<key name>
        ParameterKey=SSHLocation,ParameterValue=<SSH location>  
`
  
## Update an existing Cloudformation stack
`
aws cloudformation update-stack  
    --stack-name <name of existing stack>  
    --template-body file://<path to the template file>  
    --parameters
        ParameterKey=DBUsername,ParameterValue=<db username>
        ParameterKey=DBPassword,ParameterValue=<db password>  
        ParameterKey=EC2InstanceType,ParameterValue=<instance type>
        ParameterKey=KeyName,ParameterValue=<key name>
        ParameterKey=SSHLocation,ParameterValue=<SSH location>  
`
