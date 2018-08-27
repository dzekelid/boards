{
  "info": {
    "name": "Getty Images Remove an asset from a board",
    "_postman_id": "78170a67-de0b-4353-9878-5759d8e4c10b",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq). Use this endpoint to remove an asset from a board.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "f8bf93f2-9aa7-4ae7-a10a-aca4b0e764c2",
          "name": "Boards_RemoveAsset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/boards/:board_id/assets/:asset_id"
              ],
              "variable": [
                {
                  "id": "asset_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
                "description": "Provide access token in the format of 'Bearer {token}'",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8527d3a-1992-4b3a-be07-060a62096e66"
            }
          ]
        }
      ]
    }
  ]
}