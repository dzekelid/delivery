---
swagger: "2.0"
x-collection-name: AWS Kinesis
x-complete: 1
info:
  title: AWS Kinesis Firehose API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDeliveryStream:
    get:
      summary: Create Delivery Stream
      description: creates a delivery stream.
      operationId: CreateDeliveryStream
      x-api-path-slug: actioncreatedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: ElasticsearchDestinationConfiguration
        description: The destination in Amazon ES
        type: string
      - in: query
        name: ExtendedS3DestinationConfiguration
        description: The destination in Amazon S3
        type: string
      - in: query
        name: RedshiftDestinationConfiguration
        description: The destination in Amazon Redshift
        type: string
      - in: query
        name: S3DestinationConfiguration
        description: '[Deprecated] The destination in Amazon S3'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=DeleteDeliveryStream:
    get:
      summary: Delete Delivery Stream
      description: deletes a delivery stream and its data.
      operationId: DeleteDeliveryStream
      x-api-path-slug: actiondeletedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=DescribeDeliveryStream:
    get:
      summary: Describe Delivery Stream
      description: describes the specified delivery stream and gets the status.
      operationId: DescribeDeliveryStream
      x-api-path-slug: actiondescribedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: ExclusiveStartDestinationId
        description: The ID of the destination to start returning the destination
          information
        type: string
      - in: query
        name: Limit
        description: The limit on the number of destinations to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=ListDeliveryStreams:
    get:
      summary: List Delivery Streams
      description: lists your delivery streams.
      operationId: ListDeliveryStreams
      x-api-path-slug: actionlistdeliverystreams-get
      parameters:
      - in: query
        name: ExclusiveStartDeliveryStreamName
        description: The name of the delivery stream to start the list with
        type: string
      - in: query
        name: Limit
        description: The maximum number of delivery streams to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
---