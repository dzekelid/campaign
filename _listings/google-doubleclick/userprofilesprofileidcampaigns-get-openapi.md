---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Campaigns
  version: 1.0.0
  description: Retrieves a list of campaigns, possibly filtered. This method supports
    paging.
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