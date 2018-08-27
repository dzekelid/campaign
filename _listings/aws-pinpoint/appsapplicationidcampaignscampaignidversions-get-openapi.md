---
swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 0
info:
  title: AWS Pinpoint API Campaign Versions List
  version: 1.0.0
  description: Use the GET method to request information about your campaign versions.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/campaigns/:
    get:
      summary: Get Campaigns
      description: Campaigns are messaging initiatives that engage specific segments
        of end users. The information represented by this resource includes the segment
        that the campaign reaches out to, the message that it delivers, and the schedule
        on which it runs. You can use this resource to look up, create, update, or
        delete campaigns.
      operationId: campaigns
      x-api-path-slug: appsapplicationidcampaigns-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: An identifier used to retrieve the next page of results
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Add Campaign
      description: Use the POST method to create or update a campaign.
      operationId: addCampaign
      x-api-path-slug: appsapplicationidcampaigns-put
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /apps/application-id/campaigns/campaign-id:
    get:
      summary: Campaign Instance
      description: Use the GET method to request information about a campaign.
      operationId: getCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Update Campaign Instance
      description: Use the PUT method to update a campaign.
      operationId: updateCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-put
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    delete:
      summary: Delete Campaign Instance
      description: Use the DELETE method to delete a campaign.
      operationId: deleteCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-delete
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /apps/application-id/campaigns/campaign-id/activities:
    get:
      summary: Campaign Activities
      description: Returns information about the activity performed by a campaign,
        such as the time during which the campaign ran and the number of endpoints
        to which it delivered messages. You can use this resource to look up activity
        information by app ID and campaign ID.
      operationId: campaignActivities
      x-api-path-slug: appsapplicationidcampaignscampaignidactivities-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: token
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Activities
  /apps/application-id/campaigns/campaign-id/versions:
    get:
      summary: Campaign Versions List
      description: Use the GET method to request information about your campaign versions.
      operationId: getVersonsList
      x-api-path-slug: appsapplicationidcampaignscampaignidversions-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: token
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Versions
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