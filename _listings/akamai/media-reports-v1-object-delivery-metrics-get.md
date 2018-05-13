---
swagger: "2.0"
info:
  title: Akamai API List Object Delivery Metrics
  description: List Object Delivery Metrics
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media-reports/v1/object-delivery/metrics:
    get:
      summary: List Object Delivery Metrics
      description: List Object Delivery Metrics
      operationId: mediareportsv1objectdeliverymetrics
      responses:
        200:
          description: OK
      tags:
      - media
      - reports
      - object
      - delivery
      - metrics
definitions: []
x-collection-name: Akamai
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