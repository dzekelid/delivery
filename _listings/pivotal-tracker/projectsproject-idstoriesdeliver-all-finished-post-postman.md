{
  "info": {
    "name": "Pivotal Tracker Post Projects Project Stories Deliver All Finished",
    "_postman_id": "eed28b49-f73d-4caa-8f89-73f2448d3b92",
    "description": "Takes all finished stories and marks them as delivered. This could be used to automate a demo deploy process. The updated stories are returned as the result.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "62252a25-ff78-4f5d-90b3-313f6efb4637",
          "name": "postProjectsProjectStoriesDeliverAllFinished",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/deliver_all_finished"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Takes all finished stories and marks them as delivered. This could be used to automate a demo deploy process. The updated stories are returned as the result."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a9b0ece-47d1-423e-a177-2313ec478bc0"
            }
          ]
        }
      ]
    }
  ]
}