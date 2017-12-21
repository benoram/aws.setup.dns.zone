# Primary DNS Zone Setup
Setup Primary DNS Zone in Route53

## Prerequisites
[AWS CLI](http://docs.aws.amazon.com/rekognition/latest/dg/setup-awscli.html)

## Setup

```
aws cloudformation create-stack --stack-name aPrimaryDNSZone --template-body file://./cfn-primary-dns-zone.yaml
```
