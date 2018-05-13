{
  "info": {
    "name": "Getty Images Get Board Assets",
    "_postman_id": "f88ca6f4-5a2e-4b02-b4e6-ce42f56023cd",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq). Use this endpoint to retrieve a Board by a specific id.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "26a08fd1-039a-4a5f-b545-3d2763091aec",
          "name": "Boards_GetBoard",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/boards/:board_id"
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
              "id": "90016d34-cd3f-4ec4-a06c-6d2dcf5f140a"
            }
          ]
        }
      ]
    }
  ]
}