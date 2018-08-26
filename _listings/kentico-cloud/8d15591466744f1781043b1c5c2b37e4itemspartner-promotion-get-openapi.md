---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud Displaying the right content
  description: |-
    Retrieve one personalization variant you want to display. To learn more about retrieving content, consult the [Delivery API reference](https://developer.kenticocloud.com/reference#delivery-api).

    See <https://developer.kenticocloud.com/docs/personalizing-content#section-displaying-the-right-content> for more examples.
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /14372844-0a5d-434a-8423-605b8a631623/items:
    get:
      summary: Filtering based on date with Delivery API
      description: |-
        Filter content items directly in the API call using the `element.element_codename` query parameter and *publish from* and *publish until* elements.

        See <https://developer.kenticocloud.com/docs/scheduling-content-unpublishing#section-filtering-by-date-with-the-delivery-api> for more details.
      operationId: 143728440a5d434a8423605b8a631623ItemsGet
      x-api-path-slug: 143728440a5d434a8423605b8a631623items-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: elements.publish_until[gt]
      - in: query
        name: system.type
      responses:
        200:
          description: OK
      tags:
      - Filtering
      - Based
      - "On"
      - Date
      - Delivery
      - API
  /8d155914-6674-4f17-8104-3b1c5c2b37e4/items/partner_promotion:
    get:
      summary: Displaying the right content
      description: |-
        Retrieve one personalization variant you want to display. To learn more about retrieving content, consult the [Delivery API reference](https://developer.kenticocloud.com/reference#delivery-api).

        See <https://developer.kenticocloud.com/docs/personalizing-content#section-displaying-the-right-content> for more examples.
      operationId: 8d15591466744f1781043b1c5c2b37e4ItemsPartnerPromotionGet
      x-api-path-slug: 8d15591466744f1781043b1c5c2b37e4itemspartner-promotion-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Displaying
      - Right
      - Content
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