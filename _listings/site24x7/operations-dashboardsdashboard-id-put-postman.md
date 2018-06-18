{
  "info": {
    "name": "Operation Dashboard API Update Operations Dashboard",
    "_postman_id": "3e9f8974-af4a-4b6c-9065-3ed5604981a3",
    "description": "Update the configuration of an existing Operations Dashboard.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Operation Dashboards",
      "item": [
        {
          "id": "9f053c4c-7f6d-4137-aa6b-d510d6133705",
          "name": "create-operations-dashboard",
          "request": {
            "url": "http://www.site24x7.com./operations_dashboards?display_name\n        \n        \n            required\n            Display name for the Operations Dashboard.\n        \n    \n    \n        \n        layout_type\n        \n        \n            required\n            Layout to be used for the Operations Dashboa=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Operations Dashboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cf101e7-d601-439c-9e64-babea9eea94b"
            }
          ]
        },
        {
          "id": "fd9862c9-ed82-476b-a1e8-f640fd8f49ef",
          "name": "update-operations-dashboard",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "operations_dashboards/:dashboard_id"
              ],
              "query": [
                {
                  "key": "display_name\n        \n        \n            required\n            Display name for the Operations Dashboard.\n        \n    \n    \n        \n        layout_type\n        \n        \n            required\n            Layout to be used for the Operations Dashboa",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "dashboard_id",
                  "value": "dashboard_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the configuration of an existing Operations Dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c554fbb6-59fd-4b5c-ab56-d9ecc4598a92"
            }
          ]
        }
      ]
    }
  ]
}