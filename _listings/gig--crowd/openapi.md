---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/{requestId}/condition/delivery:
    get:
      summary: Get Request Requestid Condition Delivery
      description: Get request requestid condition delivery.
      operationId: getApiV1RequestRequestConditionDelivery
      x-api-path-slug: apiv1requestrequestidconditiondelivery-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Delivery
    post:
      summary: Post Request Requestid Condition Delivery
      description: Post request requestid condition delivery.
      operationId: postApiV1RequestRequestConditionDelivery
      x-api-path-slug: apiv1requestrequestidconditiondelivery-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Delivery
---