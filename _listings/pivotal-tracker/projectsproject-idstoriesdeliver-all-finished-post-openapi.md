---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 0
info:
  title: Pivotal Tracker Post Projects Project Stories Deliver All Finished
  description: Takes all finished stories and marks them as delivered. This could
    be used to automate a demo deploy process. The updated stories are returned as
    the result.
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{PROJECT_ID}/stories/deliver_all_finished:
    post:
      summary: Post Projects Project Stories Deliver All Finished
      description: Takes all finished stories and marks them as delivered. This could
        be used to automate a demo deploy process. The updated stories are returned
        as the result.
      operationId: postProjectsProjectStoriesDeliverAllFinished
      x-api-path-slug: projectsproject-idstoriesdeliver-all-finished-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - Deliver
      - ""
      - Finished
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