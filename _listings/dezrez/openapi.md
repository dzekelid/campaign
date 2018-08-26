---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/analytics/unlinktemplate/{templateId}:
    post:
      summary: Updates or Creates a Campaign
      description: Updates or creates a campaign.
      operationId: Analytics_UpdateGoogleCampaignBytemplateId
      x-api-path-slug: apianalyticsunlinktemplatetemplateid-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: templateId
      responses:
        200:
          description: OK
      tags:
      - S
      - Creates
      - Campaign
  /api/analytics/delete/{id}:
    delete:
      summary: Updates or Creates a Campaign
      description: Updates or creates a campaign.
      operationId: Analytics_DeleteCampaignByid
      x-api-path-slug: apianalyticsdeleteid-delete
      parameters:
      - in: path
        name: id
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
  /api/documentgeneration/templatesusinganalytics/{analyticsId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency and to
        a particular google analyitics campaign
      description: Returns a list of lettertemplates associated to this agency and
        to a particular google analyitics campaign.
      operationId: DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId
      x-api-path-slug: apidocumentgenerationtemplatesusinganalyticsanalyticsid-get
      parameters:
      - in: path
        name: analyticsId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - To
      - Particular
      - Google
      - Analyitics
      - Campaign
---