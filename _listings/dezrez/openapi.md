swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/boardordernew:
    post:
      summary: Generates an board ordering New correspondence
      description: Generates an board ordering new correspondence.
      operationId: DocumentGeneration_BoardOrderingNewPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordernew-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - New
      - Correspondence
  /api/documentgeneration/boardorderreplace:
    post:
      summary: Generates an board ordering Replace correspondence
      description: Generates an board ordering replace correspondence.
      operationId: DocumentGeneration_BoardOrderReplacePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderreplace-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - Replace
      - Correspondence
  /api/documentgeneration/boardordertakedown:
    post:
      summary: Generates an board ordering Takedown correspondence
      description: Generates an board ordering takedown correspondence.
      operationId: DocumentGeneration_BoardOrderTakedownPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordertakedown-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - Takedown
      - Correspondence
  /api/documentgeneration/boardorderupdate:
    post:
      summary: Generates an board ordering Update correspondence
      description: Generates an board ordering update correspondence.
      operationId: DocumentGeneration_BoardOrderUpdatePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderupdate-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - ""
      - Correspondence
  /api/role/{id}/boardrequest:
    post:
      summary: To send an board request email to a external provider
      description: To send an board request email to a external provider.
      operationId: Role_BoardRequestByidByupdateBoardRequestDataContract
      x-api-path-slug: apiroleidboardrequest-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateBoardRequestDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Board
      - Request
      - Email
      - To
      - External
      - Provider