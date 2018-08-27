---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Campaign Events
  description: Get Campaign Events
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/campaigns:
    post:
      summary: Add Campaign
      description: Add Campaign
      operationId: add-campaign
      x-api-path-slug: usernamecampaigns-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /{username}/campaigns/{campaign-id}:
    delete:
      summary: Delete Campaign
      description: Delete Campaign
      operationId: delete-campaign
      x-api-path-slug: usernamecampaignscampaignid-delete
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
    get:
      summary: Get Campaign
      description: Get Campaign
      operationId: get-campaign
      x-api-path-slug: usernamecampaignscampaignid-get
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Update Campaign
      description: Update Campaign
      operationId: update-campaign
      x-api-path-slug: usernamecampaignscampaignid-put
      parameters:
      - in: path
        name: campaign-id
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /{username}/campaigns/{campaign-id}/events/:
    get:
      summary: Get Campaign Events
      description: Get Campaign Events
      operationId: get-campaign-events
      x-api-path-slug: usernamecampaignscampaignidevents-get
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
      - Events
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