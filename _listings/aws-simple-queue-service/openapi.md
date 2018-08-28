---
swagger: "2.0"
x-collection-name: AWS Simple Queue Service
x-complete: 1
info:
  title: AWS Simple Queue Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SendMessage:
    get:
      summary: Send Message
      description: Delivers a message to the specified queue.
      operationId: sendMessage
      x-api-path-slug: actionsendmessage-get
      parameters:
      - in: query
        name: DelaySeconds
        description: The number of seconds to delay a specific message
        type: string
      - in: query
        name: |-
          MessageAttribute
                      , MessageAttribute.N.Name (key), MessageAttribute.N.Value (value)
        description: Each message attribute consists of a Name, Type, and Value
        type: string
      - in: query
        name: MessageBody
        description: The message to send
        type: string
      - in: query
        name: MessageDeduplicationId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: MessageGroupId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to which a message is sent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=SendMessageBatch:
    get:
      summary: Send Message Batch
      description: Delivers up to ten messages to the specified queue.
      operationId: sendMessageBatch
      x-api-path-slug: actionsendmessagebatch-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to which batched messages are
          sent
        type: string
      - in: query
        name: SendMessageBatchRequestEntry.N
        description: A list of                      SendMessageBatchRequestEntry                   items
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
---