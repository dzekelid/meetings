---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Scheduled Meetings [Beta]
  description: |-
    Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Light
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting:
    get:
      summary: Get Scheduled Meetings [Beta]
      description: |-
        Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.
        App Permission
        Meetings
        User Permission
        Meetings
        Usage Plan Group
        Light
      operationId: listMeetings
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeeting-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Scheduled
      - Meetings
      - '[Beta]'
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