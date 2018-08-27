---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Updates or Creates a Campaign
  version: 1.0.0
  description: Updates or creates a campaign.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/analytics/saveorupdategoogle:
    post:
      summary: Updates or Creates a Campaign
      description: Updates or creates a campaign.
      operationId: Analytics_UpdateGoogleCampaignBycampaign
      x-api-path-slug: apianalyticssaveorupdategoogle-post
      parameters:
      - in: body
        name: campaign
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Creates
      - Campaign
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