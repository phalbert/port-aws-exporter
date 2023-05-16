# Port AWS Exporter

Port is the Developer Platform meant to supercharge your DevOps and Developers, and allow you to regain control of your environment.


## Installation & Usage Docs

- [Port Docs](https://docs.getport.io/build-your-software-catalog/sync-data-to-catalog/aws/)


## Fetch, tail, and filter Lambda function logs

To simplify troubleshooting, SAM CLI has a command called `sam logs`, that lets you fetch logs generated by your deployed Lambda function from the command line. In addition to printing the logs on the terminal, this command has several nifty features to help you quickly find the bug.

```bash
port-aws-exporter$ sam logs --stack-name serverlessrepo-port-aws-exporter --tail
```

You can find more information and examples about filtering Lambda function logs in the [SAM CLI Documentation](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-logging.html).


## Cleanup

To delete the sample application that you created, use the AWS CLI. Assuming you used your project name for the stack name, you can run the following:

```bash
aws cloudformation delete-stack --stack-name port-aws-exporter
```