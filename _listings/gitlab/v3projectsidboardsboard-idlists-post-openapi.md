---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Boards Board Lists
  version: 1.0.0
  description: This feature was introduced in 8.13
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/boards:
    get:
      summary: Get Projects Boards
      description: This feature was introduced in 8.13
      operationId: getV3ProjectsIdBoards
      x-api-path-slug: v3projectsidboards-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
  /v3/projects/{id}/boards/{board_id}/lists:
    get:
      summary: Get Projects Boards Board Lists
      description: Does not include `backlog` and `done` lists. This feature was introduced
        in 8.13
      operationId: getV3ProjectsIdBoardsBoardIdLists
      x-api-path-slug: v3projectsidboardsboard-idlists-get
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
    post:
      summary: Post Projects Boards Board Lists
      description: This feature was introduced in 8.13
      operationId: postV3ProjectsIdBoardsBoardIdLists
      x-api-path-slug: v3projectsidboardsboard-idlists-post
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: label_id
        description: The ID of an existing label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
  /v3/projects/{id}/boards/{board_id}/lists/{list_id}:
    get:
      summary: Get Projects Boards Board Lists List
      description: Get projects boards board lists list.
      operationId: getV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-get
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
    put:
      summary: Put Projects Boards Board Lists List
      description: Put projects boards board lists list.
      operationId: putV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-put
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a list
      - in: formData
        name: position
        description: The position of the list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
    delete:
      summary: Delete Projects Boards Board Lists List
      description: Delete projects boards board lists list.
      operationId: deleteV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-delete
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a board list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
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