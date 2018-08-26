---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral End Meeting
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
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
    post:
      summary: Create Meetings [Beta]
      description: "Creates a new meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [schedule] value is invalid\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: createMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeeting-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - '[Beta]'
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/{meetingId}:
    get:
      summary: Get Meeting Info [Beta]
      description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for
        parameter [meetingId] is not found"
      operationId: loadMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Info
      - '[Beta]'
    put:
      summary: Update Meeting
      description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [password]
        value is invalid\n\n\n404\nCMN-102\nResource for parameter [extensionId] is
        not found"
      operationId: updateMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
    delete:
      summary: Delete Meeting
      description: |-
        Deletes a scheduled meeting.
        App Permission
        Meetings
        User Permission
        Meetings
        Usage Plan Group
        Medium
      operationId: deleteMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/{meetingId}/end:
    post:
      summary: End Meeting
      description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for
        parameter [meetingId] is not found"
      operationId: endMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - End
      - Meeting
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/service-info:
    get:
      summary: Get Meeting Service Info
      description: "Returns information on dial-in numbers for meetings, support and
        international dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to
        call this API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [Meetings] permission
        for requested resource."
      operationId: loadMeetingServiceInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
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
      - Meeting
      - Service
      - Info
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