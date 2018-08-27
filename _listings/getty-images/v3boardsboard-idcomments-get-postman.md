{
  "info": {
    "name": "Getty Images Get comments from a board",
    "_postman_id": "d730977e-f8da-4886-be0f-1f50aa10f7e4",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq). Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "aa2c3b2b-b7a3-42fa-81fa-6efd5016089a",
          "name": "Boards_GetComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/boards/:board_id/comments"
              ],
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
              "id": "5b610b2b-addd-4ace-ac06-0be4835a48e9"
            }
          ]
        }
      ]
    }
  ]
}