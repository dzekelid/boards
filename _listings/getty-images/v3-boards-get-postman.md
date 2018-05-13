{
  "info": {
    "name": "Getty Images Get All Boards",
    "_postman_id": "b19701a0-8cd4-4cfb-b997-5c24aa35247b",
    "description": "Boards are where you collect, curate, collaborate on and manage photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq). Use this endpoint to retrieve all Boards available for a user.\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "34617c6c-8329-47f5-a5a7-a4cc487e4b71",
          "name": "Boards_GetAllBoards",
          "request": {
            "url": "http://api.gettyimages.com/v3/boards?board_relationship=%7B%7D&page=%7B%7D&pageSize=%7B%7D&sort_order=%7B%7D",
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
              "id": "0757ef1f-82d0-4014-a0ff-50e8c397f602"
            }
          ]
        }
      ]
    }
  ]
}