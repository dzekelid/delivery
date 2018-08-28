---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Update Account Deliver Service
  description: sets which device Twitter delivers updates to for user
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/update_delivery_device:
    post:
      summary: Update Account Deliver Service
      description: sets which device Twitter delivers updates to for user
      operationId: sets-which-device-twitter-delivers-updates-to-for-user
      x-api-path-slug: accountupdate-delivery-device-post
      parameters:
      - in: query
        name: device
        description: must be one of sms, none
      - in: query
        name: include_entities
        description: whether or not to include entities
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
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