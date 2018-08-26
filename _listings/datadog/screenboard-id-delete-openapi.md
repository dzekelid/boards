---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 0
info:
  title: DataDog API Delete Screen Board
  version: 1.0.0
  description: Delete an existing screenboard.
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /screen/:board_id:
    put:
      summary: Put Screen Board
      description: PUT screen board
      operationId: putScreenBoard
      x-api-path-slug: screenboard-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
    delete:
      summary: Delete Screen Board
      description: Delete an existing screenboard.
      operationId: deleteScreenBoard
      x-api-path-slug: screenboard-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
    get:
      summary: Get Screen Board
      description: Fetch an existing screenboard's definition.
      operationId: getScreenBoard
      x-api-path-slug: screenboard-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
  /screen/share/:board_id:
    get:
      summary: Get Screen Share Board
      description: Share an existing screenboard's with a public URL.
      operationId: getScreenShareBoard
      x-api-path-slug: screenshareboard-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Share
      - Board
    delete:
      summary: Delete Screen Share Board
      description: Revoke a currently shared screenboard's.
      operationId: deleteScreenShareBoard
      x-api-path-slug: screenshareboard-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Share
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