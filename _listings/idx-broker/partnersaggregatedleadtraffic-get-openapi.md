---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Get Partners Aggregated Lead Traffic
  description: Get a list of all leads traffic history.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /leads/leadtraffic/{leadId}:
    get:
      summary: Get Leads Lead Traffic
      description: Get information on a lead's traffic history.
      operationId: LeadsLeadtrafficByLeadIdGet
      x-api-path-slug: leadsleadtrafficleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
      - Traffic
  /partners/aggregatedleadtraffic:
    get:
      summary: Get Partners Aggregated Lead Traffic
      description: Get a list of all leads traffic history.
      operationId: PartnersAggregatedleadtrafficGet
      x-api-path-slug: partnersaggregatedleadtraffic-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Lead
      - Traffic
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