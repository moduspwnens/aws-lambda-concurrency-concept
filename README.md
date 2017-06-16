# AWS Lambda Concurrency Concept

A proof of concept for a method of invoking an AWS Lambda function hundreds or thousands of times with a single API call.

### Background

See my post on Medium [here](https://medium.com/@bennlinger/massively-parallel-sqs-processing-f0c1ea8f39eb) for how it works and why.

### Deploy

It only takes a few clicks. Just log into your AWS account (with appropriate permissions) and click this button:

[![Launch Stack](/launch-stack-button.png?raw=true "Launch Stack")](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=aws-lambda-fan-out-ui&templateURL=https://s3.amazonaws.com/bennlinger-public/lambda-fan-out-concept-20170616/lambda-fan-out-ui.yaml)

Simply click "Next" until you get to the **Review** page, then check the box for *I acknowledge that AWS CloudFormation might create IAM resources.* and click **Create**.

The stack is now being created. It typically takes 5-7 minutes to finish. Use the refresh button (⟳) to check on it periodically. Once it reaches a **CREATE_COMPLETE** state, it's ready to go! Simply select the stack, click the *Outputs* tab, and click the link next to the one called **DemoUrl**.

### Destroy

To delete all the resources, simply delete the stack.