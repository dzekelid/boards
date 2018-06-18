{
  "info": {
    "name": "Operation Dashboard API Create Operations Dashboard",
    "_postman_id": "35e07104-b9e2-47e7-90a2-e1095905f309",
    "description": "Create a new Operations Dashboard",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Operation Dashboards",
      "item": [
        {
          "id": "157f8766-4601-4f19-b37c-ac7a60799493",
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
              "id": "10264809-941f-473d-bec4-e46fbca9dca1"
            }
          ]
        }
      ]
    }
  ]
}