{
  "info": {
    "name": "Getty Images Add an asset to a board",
    "_postman_id": "d1dc94b2-781f-4ae1-9578-6eb2bdeb7042",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place.\r\nMore information on the [Boards FAQ](http://www.gettyimages.com/boards/faq). Use this endpoint to add an asset to a board.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "f32b0445-79ec-41c6-aafb-3d37c1e5a7aa",
          "name": "Boards_AddAsset",
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
            "method": "PUT",
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
              "id": "79d92966-3131-4879-9793-bd7197d8f594"
            }
          ]
        }
      ]
    }
  ]
}