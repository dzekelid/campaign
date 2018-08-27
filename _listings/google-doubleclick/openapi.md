swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/campaigns:
    get:
      summary: Get Campaigns
      description: Retrieves a list of campaigns, possibly filtered. This method supports
        paging.
      operationId: dfareporting.campaigns.list
      x-api-path-slug: userprofilesprofileidcampaigns-get
      parameters:
      - in: query
        name: advertiserGroupIds
        description: Select only campaigns whose advertisers belong to these advertiser
          groups
      - in: query
        name: advertiserIds
        description: Select only campaigns that belong to these advertisers
      - in: query
        name: archived
        description: Select only archived campaigns
      - in: query
        name: atLeastOneOptimizationActivity
        description: Select only campaigns that have at least one optimization activity
      - in: query
        name: excludedIds
        description: Exclude campaigns with these IDs
      - in: query
        name: ids
        description: Select only campaigns with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: overriddenEventTagId
        description: Select only campaigns that have overridden this event tag ID
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for campaigns by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only campaigns that belong to this subaccount
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    patch:
      summary: Update Campaign
      description: Updates an existing campaign. This method supports patch semantics.
      operationId: dfareporting.campaigns.patch
      x-api-path-slug: userprofilesprofileidcampaigns-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    post:
      summary: Create Campaign
      description: Inserts a new campaign.
      operationId: dfareporting.campaigns.insert
      x-api-path-slug: userprofilesprofileidcampaigns-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: defaultLandingPageName
        description: Default landing page name for this new campaign
      - in: query
        name: defaultLandingPageUrl
        description: Default landing page URL for this new campaign
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    put:
      summary: Update Campaign
      description: Updates an existing campaign.
      operationId: dfareporting.campaigns.update
      x-api-path-slug: userprofilesprofileidcampaigns-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
  /userprofiles/{profileId}/campaigns/{id}:
    get:
      summary: Get Campaign
      description: Gets one campaign by ID.
      operationId: dfareporting.campaigns.get
      x-api-path-slug: userprofilesprofileidcampaignsid-get
      parameters:
      - in: path
        name: id
        description: Campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign