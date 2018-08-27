{
  "info": {
    "name": "GitLab Get Projects Boards",
    "_postman_id": "2e8cc541-63ea-4676-a5f1-d6d95412f261",
    "description": "This feature was introduced in 8.13",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "39b5f3af-3359-4939-9be7-dcdafea884a6",
          "name": "getV3ProjectsIdBoards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This feature was introduced in 8.13"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23e22417-5a05-449e-a41c-93b56492d582"
            }
          ]
        }
      ]
    }
  ]
}