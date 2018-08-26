---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Meetings
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToMeeting - Upcoming meetings by group
  x-api-slug: groupsgroupkeyupcomingmeetings-get
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-openapi.md
- name: GoToMeeting - Historical meetings
  x-api-slug: historicalmeetings-get
  description: 'Get historical meetings for the currently authenticated organizer
    that started within the specified date/time range. Remark: Meetings which are
    still ongoing at the time of the request are NOT contained in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/historicalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/historicalmeetings-get-openapi.md
- name: GoToMeeting - Upcoming meetings
  x-api-slug: upcomingmeetings-get
  description: Gets upcoming meetings for the current authenticated organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/upcomingmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/upcomingmeetings-get-openapi.md
- name: GoToMeeting - Historical meetings by organizer
  x-api-slug: organizersorganizerkeyhistoricalmeetings-get
  description: Get historical meetings for the specified organizer that started within
    the specified date/time range. Meetings which are still ongoing at the time of
    the request are not included in the result.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizersorganizerkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizersorganizerkeyhistoricalmeetings-get-openapi.md
- name: GoToMeeting - Historical meetings by group
  x-api-slug: groupsgroupkeyhistoricalmeetings-get
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: GoToMeeting - Attendees by meeting
  x-api-slug: meetingsmeetinginstancekeyattendees-get
  description: List all attendees for specified meetingId of historical meeting. The
    historical meetings can be fetched using 'Get historical meetings', 'Get historical
    meetings by organizer', and 'Get historical meetings by group'. For users with
    the admin role this call returns attendees for any meeting. For any other user
    the call will return attendees for meetings on which the user is a valid organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-openapi.md
- name: GoToMeeting - Attendees by meeting
  x-api-slug: meetingsmeetinginstancekeyattendees-get
  description: List all attendees for specified meetingId of historical meeting. The
    historical meetings can be fetched using 'Get historical meetings', 'Get historical
    meetings by organizer', and 'Get historical meetings by group'. For users with
    the admin role this call returns attendees for any meeting. For any other user
    the call will return attendees for meetings on which the user is a valid organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-openapi.md
- name: GoToWebinar API - Get webinar meeting times
  x-api-slug: organizerkeywebinarswebinarkeymeetingtimes-get
  description: Get webinar meeting times.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizerkeywebinarswebinarkeymeetingtimes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizerkeywebinarswebinarkeymeetingtimes-get-openapi.md
- name: GoToWebinar API - Get webinar meeting times
  x-api-slug: organizerkeywebinarswebinarkeymeetingtimes-get
  description: Get webinar meeting times.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizerkeywebinarswebinarkeymeetingtimes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/logmein/organizerkeywebinarswebinarkeymeetingtimes-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---