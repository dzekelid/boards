{
  "info": {
    "name": "Plentymarkets Lists all boards.",
    "_postman_id": "94053890-6c25-469e-acdf-e1d7a1743827",
    "description": "Lists all boards..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "1b4c8c55-7118-4a88-8c57-3545ec3952ec",
          "name": "getRestBoards",
          "request": {
            "url": "http://example.com/rest/boards",
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
            "description": "Lists all boards.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f7dd313-bf04-40c6-87ed-7090f6bebc2b"
            }
          ]
        }
      ]
    }
  ]
}