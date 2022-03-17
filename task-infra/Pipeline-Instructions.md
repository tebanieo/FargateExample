Run the following AWS CLI command to create your first pipeline:

```bash
aws cloudformation create-stack \
    --stack-name fargateexample-pipeline \
    --template-body file://pipeline.yaml \
    --capabilities CAPABILITY_NAMED_IAM
```

Response type
```json
{
    "StackId": "arn:aws:cloudformation:ap-southeast-2:680285499255:stack/fargateexample-pipeline/ead56740-a59f-11ec-a43b-0a15eb7555ce"
}
```

```bash
aws cloudformation update-stack \
    --stack-name fargateexample-pipeline \
    --template-body file://pipeline.yaml \
    --capabilities CAPABILITY_NAMED_IAM
```