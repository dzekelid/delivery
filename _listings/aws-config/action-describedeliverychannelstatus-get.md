---
swagger: "2.0"
info:
  title: AWS Config API Describe Delivery Channel Status
  version: 1.0.0
  description: Returns the current status of the specified delivery channel.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDeliveryChannelStatus:
    get:
      summary: ' Describe Delivery Channel Status '
      description: Returns the current status of the specified delivery channel
      operationId: describeDeliveryChannelStatus
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - delivery channels
definitions: []
x-collection-name: AWS Config
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