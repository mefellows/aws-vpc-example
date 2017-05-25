# AWS VPC Creation


Validate the Stack:

```
aws --profile dius-dev --region us-east-1 cloudformation validate-template --template-body file://infra.json
```

Create Stack:

```
aws --profile dius-dev --region us-east-1 cloudformation create-stack --stack-name mfellows-aws-cert --template-body file://infra.json --disable-rollback
```

Describe Stack:

```
aws --profile dius-dev --region us-east-1 cloudformation describe-stacks --stack-name mfellows-aws-cert
```

Update Stack:

```
aws --profile dius-dev --region us-east-1 cloudformation update-stack --stack-name mfellows-aws-cert --template-body file://infra.json
```