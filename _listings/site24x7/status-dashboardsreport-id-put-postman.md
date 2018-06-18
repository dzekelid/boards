{
  "info": {
    "name": "Status Dashboard API Update Status Dashboard",
    "_postman_id": "de6ddcac-80c6-4275-b6d3-8d77ec455085",
    "description": "Update the configuration of an existing Status Dashboard.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Status Dashboards",
      "item": [
        {
          "id": "a9f7b106-f5f6-4d6b-a24d-a727a54deaba",
          "name": "create-status-dashboard",
          "request": {
            "url": "http://www.site24x7.com./status_dashboards?display_name\n        \n        \n            required\n            Display name for the Status Dashboard.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Status Dashboard.=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Status Dashboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9567b909-ea4f-447d-bee3-c550560e0362"
            }
          ]
        },
        {
          "id": "e45ef6fd-9cc5-454d-a213-cf7ac8523ff9",
          "name": "update-status-dashboard",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "status_dashboards/:report_id"
              ],
              "query": [
                {
                  "key": "display_name\n        \n        \n            required\n            Display name for the Status Dashboard.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Status Dashboard.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_id",
                  "value": "report_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the configuration of an existing Status Dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0051876-2b80-4684-8a79-1b32d429cf84"
            }
          ]
        }
      ]
    }
  ]
}