{
  "info": {
    "name": "Status Dashboard API Create Status Dashboard",
    "_postman_id": "5fb729d4-743b-43d3-b5ff-67800512471c",
    "description": "Create a new Status Dashboard",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Status Dashboards",
      "item": [
        {
          "id": "afa766e3-d22e-4fda-8e04-1a4f5844e709",
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
              "id": "434b14c8-5310-4c02-b414-0b62c13fe4ba"
            }
          ]
        }
      ]
    }
  ]
}