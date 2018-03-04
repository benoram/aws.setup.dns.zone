# Primary DNS Zone Setup
Setup DNS Zone in Route53

## Prerequisites
[AWS CLI](https://docs.aws.amazon.com/cli/latest/reference/)

## Setup
This deploys a CloudFormation script to us-east-1 to setup the domain. 

```
TEMP_DOMAINNAME='Domain.com'
aws cloudformation create-stack --stack-name aPrimaryDNSZone --template-body file://./cfn-dns-zone.yaml --region us-east-1 --parameters ParameterKey=Domain,ParameterValue=$TEMP_DOMAINNAME
```
