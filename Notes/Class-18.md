# AWS: Events

## AWS SQS vs SNS

**What is the difference betweeen SQS and SNS?**

- SNS is a distributed publish-subscribe service.

- SQS is distributed queuing service.

**What are some use cases for both SNS and SQS?**

- Granting AWS account access to a topic in Amazon SNS.
- Limiting subscriptions to HTTPS.
- Publishing messages to an Amazon SQS queue.
- Allowing Amazon S3 event notifications to publish to a topic.
- Allowing Amazon SES to publish to a topic that is owned by another account.
- Coupling SQS and SNS to work together, such as in a Fanout scenario which
- requires asynchronous processing of messages.

## AWS SNS and SQS

**Describe how to use SQS and SNS in a “fanout” pattern.**

- When using the "fanout" pattern with SQS and SNS, you publish a message to the SNS topic, and SNS will deliver the message to all the subscribed SQS queues, allowing each subscriber to consume and process the messages independently. This pattern is useful when you need to broadcast messages to multiple consumers in a scalable and decoupled manner.

**Explain how “push notifications” work, using SNS.**

- With SNS, push notifications are facilitated by publishing messages to an SNS topic, and those messages are then immediately delivered to all registered subscribers or endpoints, enabling real-time communication and updates.

## SQS and SNS Basics

**How might a large scale, distributed application make use of a Queue system like SQS?**

- SQS is a powerful tool for large-scale distributed applications, enabling decoupling, scalability, fault tolerance, and efficient message processing to ensure smooth and reliable operation in dynamic and demanding environments.
