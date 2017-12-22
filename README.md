# Primary DNS Zone Setup
Setup Primary DNS Zone in Route53

## Prerequisites
[AWS CLI](http://docs.aws.amazon.com/rekognition/latest/dg/setup-awscli.html)

## Setup
This deploys a CloudFormation script to us-east-1 to setup the domain. 

```
TEMP_DOMAINNAME='Domain.com'
aws cloudformation create-stack --stack-name aPrimaryDNSZone --template-body file://./cfn-primary-dns-zone.yaml --region us-east-1 --parameters ParameterKey=Domain,ParameterValue=$TEMP_DOMAINNAME
```
