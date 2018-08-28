---
swagger: "2.0"
x-collection-name: AWS Simple Queue Service
x-complete: 0
info:
  title: AWS Simple Queue Service API Send Message
  version: 1.0.0
  description: Delivers a message to the specified queue.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---