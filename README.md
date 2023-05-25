# lambda-v2
aws lambda in golang with SNS integration

## Design
- producer->events->consumed
- lambda will produce and emit events onto SQS queues and publish notifications to SNS topics
- init function establishes global state
- intit function helps establish client connections as the lambda is booting up

1. go mod init github.com/robertocamp/lambda-v2
2. 