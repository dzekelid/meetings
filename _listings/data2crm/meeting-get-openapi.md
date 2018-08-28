---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM GET for Meeting
  description: Returns all meetings from the system
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /meeting/{meeting_id}:
    delete:
      summary: DELETE for Meeting
      description: Delete meeting information
      operationId: deleteMeetingEntity
      x-api-path-slug: meetingmeeting-id-delete
      parameters:
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
    get:
      summary: GET for Meeting
      description: Return meeting information
      operationId: getMeetingEntity
      x-api-path-slug: meetingmeeting-id-get
      parameters:
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
    put:
      summary: PUT for Meeting
      description: Update meeting information
      operationId: updateMeetingEntity
      x-api-path-slug: meetingmeeting-id-put
      parameters:
      - in: body
        name: body
        description: Update meeting information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
  /meeting:
    get:
      summary: GET for Meeting
      description: Returns all meetings from the system
      operationId: getMeetingCollection
      x-api-path-slug: meeting-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
    post:
      summary: POST for Meeting
      description: Add meeting into the system
      operationId: createMeetingEntity
      x-api-path-slug: meeting-post
      parameters:
      - in: body
        name: body
        description: Add meeting into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
  /meeting/count:
    get:
      summary: COUNT for Meeting
      description: Count all meetings from the system
      operationId: getMeetingCountCollection
      x-api-path-slug: meetingcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Count
  /meeting/describe:
    get:
      summary: DESCRIBE for Meeting
      description: Returns describe for meetings
      operationId: getMeetingDescribe
      x-api-path-slug: meetingdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Describe
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