---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Patch Campaigns Campaign
  description: |-
    Update a campaign. This is especially useful if you only set up the campaign using POST /campaigns, but didn't set many of the parameters.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaigns/{campaign_id}:
    delete:
      summary: Delete Campaigns Campaign
      description: |-
        **This endpoint allows you to delete a specific campaign.**

        Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.delete
      x-api-path-slug: campaignscampaign-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
    get:
      summary: Get Campaigns Campaign
      description: |-
        **This endpoint allows you to retrieve a specific campaign.**

        Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.get
      x-api-path-slug: campaignscampaign-id-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
    patch:
      summary: Patch Campaigns Campaign
      description: |-
        Update a campaign. This is especially useful if you only set up the campaign using POST /campaigns, but didn't set many of the parameters.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.patch
      x-api-path-slug: campaignscampaign-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
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