{
  "info": {
    "name": "Getty Images Remove Assets From Board",
    "_postman_id": "9f894725-de20-4ad5-9850-91b1a8ba1f02",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse this endpoint to remove a set of assets from a board.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "98d9a536-fdc6-4b87-babd-9fd2b384311f",
          "name": "Boards_RemoveAssets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/boards/:board_id/assets"
              ],
              "query": [
                {
                  "key": "asset_ids",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
              "id": "d89f9885-d1ed-4cd0-9849-a4492e9760e5"
            }
          ]
        }
      ]
    }
  ]
}