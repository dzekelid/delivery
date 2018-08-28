---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
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
---