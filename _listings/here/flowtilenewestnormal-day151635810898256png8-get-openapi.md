---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Traffic API Transparent Traffic Map
  description: |-
    *Request a transparent tile with traffic flow information*

    To obtain a transparent map tile displaying traffic flow, use the `flowtile` parameter in the path of the request URL.



    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  version: 1.0.0
host: tiles.traffic.cit.api.here.com
basePath: /traffic/6.0/tiles/8/133/86/256
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flowtile/newest/normal.day/15/16358/10898/256/png8:
    get:
      summary: Transparent Traffic Map
      description: |-
        *Request a transparent tile with traffic flow information*

        To obtain a transparent map tile displaying traffic flow, use the `flowtile` parameter in the path of the request URL.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: FlowtileNewestNormalDay151635810898256Png8Get
      x-api-path-slug: flowtilenewestnormal-day151635810898256png8-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      responses:
        200:
          description: OK
      tags:
      - Transparent
      - Traffic
      - Map
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