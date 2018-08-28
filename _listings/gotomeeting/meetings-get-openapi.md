---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: 'Go To Meeting DEPRECATED: Get historical meetings'
  description: 'DEPRECATED: Please use the new API calls ''Get historical meetings''
    and ''Get upcoming meetings''.  Gets historical meetings for the current authenticated
    organizer. Requires date range for filtering results to only meetings within specified
    dates. History searches will contain the parameter ''meetingInstanceKey'' which
    is used in conjunction with the call ''Get Attendees by Meeting'' to get attendee
    information for a past meeting.'
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