AWS-SNS-To-Slack-hook
===
Use AWS Lambda to forward message to Slack from SNS

## Preparing
* Prepare the IAM Execution Role. For example:
```json
  {
    "Version": "2012-10-17",
    "Statement": [
    {
        "Effect": "Allow",
        "Action": [
          "sns:GetTopicAttributes",
          "sns:List*"
        ],
        "Resource": "*"
      }
    ]
  } 
```
* Prepare the Slack web-incoming-webhook url
  1. Create a channel for aws-sns in slack
  2. add a Incoming WebHooks service integration
  3. get the webhook url

## Create Lambda Function with js code
## AWS SNS Topic Subscription for AWS Lambda
* Select topic you want and subscirpt to it
* select AWS Lambda as Protocl and select Lambda function