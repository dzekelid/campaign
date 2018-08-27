swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaign:
    post:
      summary: Add Campaign
      description: Add a Campaign
      operationId: campaignAdd
      x-api-path-slug: campaign-post
      parameters:
      - in: formData
        name: name
        description: Name for this Campaign
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /campaign/{campaignId}:
    put:
      summary: Edit Campaign
      description: Edit an existing Campaign
      operationId: campaignEdit
      x-api-path-slug: campaigncampaignid-put
      parameters:
      - in: path
        name: campaignId
        description: The Campaign ID to Edit
      - in: formData
        name: name
        description: Name for this Campaign
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Campaign
    delete:
      summary: Delete Campaign
      description: Delete an existing Campaign
      operationId: campaignDelete
      x-api-path-slug: campaigncampaignid-delete
      parameters:
      - in: path
        name: campaignId
        description: The Campaign ID to Delete
      responses:
        200:
          description: OK
      tags:
      - Campaign