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
  /api/agency/meetingplaces:
    get:
      summary: Get meeting places for an agency
      description: Get meeting places for an agency.
      operationId: Agency_MeetingPlaces
      x-api-path-slug: apiagencymeetingplaces-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Placesan
      - Agency
  /api/agency/savemeetingplace:
    post:
      summary: Saves a new meeting place to that particular agency
      description: Saves a new meeting place to that particular agency.
      operationId: Agency_SaveMeetingPlaceBydataContract
      x-api-path-slug: apiagencysavemeetingplace-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - New
      - Meeting
      - Place
      - To
      - That
      - Particular
      - Agency
  /api/agency/tenantclause:
    get:
      summary: Get meeting places for an agency
      description: Get meeting places for an agency.
      operationId: Agency_TenantClause
      x-api-path-slug: apiagencytenantclause-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Placesan
      - Agency
  /api/documentgeneration/reschedulemeeting:
    post:
      summary: Generates a meeting letter correspondence
      description: Generates a meeting letter correspondence.
      operationId: DocumentGeneration_ReschedulMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulemeeting-post
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
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/cancelmeeting:
    post:
      summary: Generates a cancel a meeting letter correspondence
      description: Generates a cancel a meeting letter correspondence.
      operationId: DocumentGeneration_CancelMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelmeeting-post
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
      - Cancel
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/confirmmeeting:
    post:
      summary: Generates a confirm a meeting letter correspondence
      description: Generates a confirm a meeting letter correspondence.
      operationId: DocumentGeneration_ConfirmMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmmeeting-post
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
      - Confirm
      - Meeting
      - Letter
      - Correspondence