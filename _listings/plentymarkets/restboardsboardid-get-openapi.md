---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Gets a single board by its ID
  description: Gets a single board by its id.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/boards:
    get:
      summary: Lists all boards.
      description: Lists all boards..
      operationId: getRestBoards
      x-api-path-slug: restboards-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Boards
    post:
      summary: Creates a new board.
      description: Creates a new board..
      operationId: postRestBoards
      x-api-path-slug: restboards-post
      parameters:
      - in: body
        name: /rest/boards
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Board
  /rest/boards/{boardId}:
    delete:
      summary: Deletes a specific board.
      description: Deletes a specific board..
      operationId: deleteRestBoardsBoard
      x-api-path-slug: restboardsboardid-delete
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Board
    get:
      summary: Gets a single board by its ID
      description: Gets a single board by its id.
      operationId: getRestBoardsBoard
      x-api-path-slug: restboardsboardid-get
      parameters:
      - in: path
        name: boardId
      - in: query
        name: tasksPerPage
        description: Maximum number of tasks to list per column
      responses:
        200:
          description: OK
      tags:
      - S
      - Single
      - Board
      - By
      - Its
      - ID
    post:
      summary: Copies a specific board.
      description: Copies a specific board..
      operationId: postRestBoardsBoard
      x-api-path-slug: restboardsboardid-post
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Copies
      - Specific
      - Board
    put:
      summary: Updates a specific board.
      description: Updates a specific board..
      operationId: putRestBoardsBoard
      x-api-path-slug: restboardsboardid-put
      parameters:
      - in: body
        name: /rest/boards/{boardId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Board
  /rest/boards/{boardId}/columns:
    get:
      summary: Lists all columns for a given board
      description: Lists all columns for a given board.
      operationId: getRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-get
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Columnsa
      - Given
      - Board
    post:
      summary: Creates a new column and assigns it to a given board
      description: Creates a new column and assigns it to a given board.
      operationId: postRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Column
      - Assigns
      - It
      - To
      - Given
      - Board
  /rest/boards/{boardId}/columns/{columnId}/position:
    put:
      summary: Updates the position of a specific column. Also updates the positions
        of all following columns on the same board.
      description: Updates the position of a specific column. also updates the positions
        of all following columns on the same board..
      operationId: putRestBoardsBoardColumnsColumnPosition
      x-api-path-slug: restboardsboardidcolumnscolumnidposition-put
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: position
      responses:
        200:
          description: OK
      tags:
      - S
      - Position
      - Of
      - Specific
      - Column
      - ""
      - Also
      - Updates
      - Positions
      - Of
      - ""
      - Following
      - Columns
      - "On"
      - Same
      - Board
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---