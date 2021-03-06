---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Calendars
  description: List calendars Get all the user's calendars (/calendars navigation
    property), get the calendars from the default calendar group or from a specific
    calendar group.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/calendarGroup/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroup/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /me/calendarGroups/{id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupsidcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /me/calendargroups/{calendar_group_id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupscalendar-group-idcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: calendar_group_id
        type: string
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupscalendar-group-idcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: calendar_group_id
        type: string
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
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