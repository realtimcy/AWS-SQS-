Lambert Lamda SQS Demo





Ideally, this project demonstrates a simple serverless workflow using Amazon SQS and AWS Lambda

WHAT it DOES:

- (Mailbox) Messages are sent to an Amazon SQS Queue
- The Lamda Function (read\_messages) is triggered whenerver a new message is received. 
- The function processes the message by:
1. Logging the message aID and Content into CloudWatch Logs
2. By confirming how many messages were handles. 
- Once processed, the message is removed from the queue. 

The result here is that messages are picked up instantly, processed and logged out qithout any serveres to manage. 

Example:

Send any message to the SQS queue and clod logs will show: Message ID: 12345-abcd

Message Body: Hello 

Successfully processed 1 messages.


