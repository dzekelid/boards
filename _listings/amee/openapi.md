swagger: "2.0"
x-collection-name: AMEE
x-complete: 1
info:
  title: AMEE WRI Aqueduct API
  version: 1.0.0
host: api.roaring.io
basePath: /company/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /company-board-members:
    get:
      summary: Get Company Board Members
      description: Get company board members.
      operationId: getCompanyBoardMembers
      x-api-path-slug: companyboardmembers-get
      parameters:
      - in: query
        name: companyId
        description: Company identification for the company
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Board
      - Members
    post:
      summary: Post Company Board Members
      description: Post company board members.
      operationId: postCompanyBoardMembers
      x-api-path-slug: companyboardmembers-post
      parameters:
      - in: body
        name: body
        description: Request body with company identifiers to lookup
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Board
      - Members