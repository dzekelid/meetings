---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Meetings
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: 'Go To Meeting - DEPRECATED: Get historical meetings by group'
  x-api-slug: groupsgroupkeymeetings-get
  description: 'DEPRECATED: Please use the new API calls ''Get historical meetings
    by group'' and ''Get upcoming meetings by group''. Get meetings for a specified
    group. Additional filters can be used to view only meetings within a specified
    date range. This API call is only available to users with the admin role.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/groupsgroupkeymeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/groupsgroupkeymeetings-get-openapi.md
- name: 'Go To Meeting - DEPRECATED: Get historical meetings'
  x-api-slug: meetings-get
  description: 'DEPRECATED: Please use the new API calls ''Get historical meetings''
    and ''Get upcoming meetings''.  Gets historical meetings for the current authenticated
    organizer. Requires date range for filtering results to only meetings within specified
    dates. History searches will contain the parameter ''meetingInstanceKey'' which
    is used in conjunction with the call ''Get Attendees by Meeting'' to get attendee
    information for a past meeting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/meetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/meetings-get-openapi.md
- name: Go To Webinar - Get webinar meeting times
  x-api-slug: organizersorganizerkeywebinarswebinarkeymeetingtimes-get
  description: Retrieves the meeting times for a webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeymeetingtimes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeymeetingtimes-get-openapi.md
- name: Go To Webinar - Get webinar meeting times
  x-api-slug: organizersorganizerkeywebinarswebinarkeymeetingtimes-get
  description: Retrieves the meeting times for a webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeymeetingtimes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeymeetingtimes-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.url.shortener.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gotomeeting.stack.network
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---