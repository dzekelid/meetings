---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Meeting Update meeting
  description: Updates an existing meeting specified by meetingId.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/meetings:
    get:
      summary: 'DEPRECATED: Get historical meetings by group'
      description: 'DEPRECATED: Please use the new API calls ''Get historical meetings
        by group'' and ''Get upcoming meetings by group''. Get meetings for a specified
        group. Additional filters can be used to view only meetings within a specified
        date range. This API call is only available to users with the admin role.'
      operationId: deprecated-please-use-the-new-api-calls-get-historical-meetings-by-group-and-get-upcoming-meetings-b
      x-api-path-slug: groupsgroupkeymeetings-get
      parameters:
      - in: query
        name: endDate
        description: If history=true, required end of date range, in ISO8601 UTC format,
          e
      - in: query
        name: history
        description: When true, returns all past meetings within date range
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: If history=true, required start of date range, in ISO8601 UTC
          format, e
      responses:
        200:
          description: OK
      tags:
      - Groups
      - GroupKey
      - Meetings
  /meetings:
    get:
      summary: 'DEPRECATED: Get historical meetings'
      description: 'DEPRECATED: Please use the new API calls ''Get historical meetings''
        and ''Get upcoming meetings''.  Gets historical meetings for the current authenticated
        organizer. Requires date range for filtering results to only meetings within
        specified dates. History searches will contain the parameter ''meetingInstanceKey''
        which is used in conjunction with the call ''Get Attendees by Meeting'' to
        get attendee information for a past meeting.'
      operationId: deprecated-please-use-the-new-api-calls-get-historical-meetings-and-get-upcoming-meetings---gets-his
      x-api-path-slug: meetings-get
      parameters:
      - in: query
        name: endDate
        description: If history=true, required end of date range, in ISO8601 UTC format,
          e
      - in: query
        name: history
        description: When true, returns all past meetings within date range
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: If history=true, required start of date range, in ISO8601 UTC
          format, e
      responses:
        200:
          description: OK
      tags:
      - Meetings
    post:
      summary: Create meeting
      description: Create a new meeting based on the parameters specified.
      operationId: create-a-new-meeting-based-on-the-parameters-specified-
      x-api-path-slug: meetings-post
      parameters:
      - in: body
        name: body
        description: The meeting details
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
  /meetings/{meetingId}:
    delete:
      summary: Delete meeting
      description: Deletes the meeting identified by the meetingId.
      operationId: deletes-the-meeting-identified-by-the-meetingid-
      x-api-path-slug: meetingsmeetingid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
    get:
      summary: Get meeting
      description: Returns the meeting details for the specified meeting.
      operationId: returns-the-meeting-details-for-the-specified-meeting-
      x-api-path-slug: meetingsmeetingid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
    put:
      summary: Update meeting
      description: Updates an existing meeting specified by meetingId.
      operationId: updates-an-existing-meeting-specified-by-meetingid-
      x-api-path-slug: meetingsmeetingid-put
      parameters:
      - in: body
        name: body
        description: The meeting details
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
  /meetings/{meetingId}/attendees:
    get:
      summary: Get attendees by meeting
      description: List all attendees for specified meetingId of historical meeting.
        The historical meetings can be fetched using 'Get historical meetings', 'Get
        historical meetings by organizer', and 'Get historical meetings by group'.
        For users with the admin role this call returns attendees for any meeting.
        For any other user the call will return attendees for meetings on which the
        user is a valid organizer.
      operationId: list-all-attendees-for-specified-meetingid-of-historical-meeting--the-historical-meetings-can-be-fet
      x-api-path-slug: meetingsmeetingidattendees-get
      parameters:
      - in: path
        name: meetingId
        description: The meeting ID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
      - Attendees
  /meetings/{meetingId}/start:
    get:
      summary: Start meeting
      description: Returns a host URL that can be used to start a meeting. When this
        URL is opened in a web browser, the GoToMeeting client will be downloaded
        and launched and the meeting will start. The end user is not required to login
        to a client.
      operationId: returns-a-host-url-that-can-be-used-to-start-a-meeting--when-this-url-is-opened-in-a-web-browser-the
      x-api-path-slug: meetingsmeetingidstart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
      - Start
  /organizers/{organizerKey}/meetings:
    get:
      summary: 'DEPRECATED: Get meetings by organizer'
      description: 'DEPRECATED: Please use the new API calls ''Get historical meetings
        by organizer'' and ''Get upcoming meetings by organizer''. Gets future (scheduled)
        or past (history) meetings for a specified organizer. Include ''history=true''
        and the past start and end dates in the URL to retrieve past meetings. Enter
        ''scheduled=true'' (without dates) to get scheduled meetings.'
      operationId: deprecated-please-use-the-new-api-calls-get-historical-meetings-by-organizer-and-get-upcoming-meetin
      x-api-path-slug: organizersorganizerkeymeetings-get
      parameters:
      - in: query
        name: endDate
        description: If history is true, required end of date range, in ISO8601 UTC
          format, e
      - in: query
        name: history
        description: When true, returns all past meetings within date range
      - in: query
        name: No Name
      - in: query
        name: scheduled
        description: When true, returns all future meetings
      - in: query
        name: startDate
        description: If history is true, required start of date range, in ISO8601
          UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Meetings
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