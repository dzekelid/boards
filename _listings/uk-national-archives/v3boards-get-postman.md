{
  "info": {
    "name": "Getty Images Search API Get Boards",
    "_postman_id": "2f8ce44f-4d79-4ad8-b1c1-49cc83c5281d",
    "description": "<b>***beta***</b> get all boards that the user participates in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Boards",
      "item": [
        {
          "id": "14f0ef33-62c0-463d-a18d-27d58bc1d5c0",
          "name": "getV3Boards",
          "request": {
            "url": "http://api.gettyimages.com/v3/boards?board_relationship=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_order=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Provide a header to specify the language of result values",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Provide access token in the format of Bearer {token}",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "<b>***beta***</b> get all boards that the user participates in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d20236b-953a-475b-bcdb-9ebd5f1e9ac4"
            }
          ]
        }
      ]
    }
  ]
}