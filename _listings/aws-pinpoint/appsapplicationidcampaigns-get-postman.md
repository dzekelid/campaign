{
  "info": {
    "name": "AWS Pinpoint API Get Campaigns",
    "_postman_id": "a2a5e9b6-0e23-4880-91cd-0f2c04379886",
    "description": "Campaigns are messaging initiatives that engage specific segments of end users. The information represented by this resource includes the segment that the campaign reaches out to, the message that it delivers, and the schedule on which it runs. You can use this resource to look up, create, update, or delete campaigns.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaign Activities",
      "item": [
        {
          "id": "ca2fcca0-44a0-4c77-bdc8-af102673f0f2",
          "name": "campaignActivities",
          "request": {
            "url": "http://example.com/api/apps/application-id/campaigns/campaign-id/activities?page-size=page-size&token=token",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "accept",
                "description": "Specify the media type you will accept as a response:  application/json ??? A JSON response body",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the activity performed by a campaign, such as the time during which the campaign ran and the number of endpoints to which it delivered messages. You can use this resource to look up activity information by app ID and campaign ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "376ccc54-611d-48f9-9c02-685486663fcd"
            }
          ]
        }
      ]
    },
    {
      "name": "Campaign",
      "item": [
        {
          "id": "5b1c9c7b-d727-4211-a041-585e2e2371a7",
          "name": "campaigns",
          "request": {
            "url": "http://example.com/api/apps/application-id/campaigns/?page-size=page-size&token=token",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "accept",
                "description": "Specify the media type you will accept as a response:  application/json ??? A JSON response body",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Campaigns are messaging initiatives that engage specific segments of end users. The information represented by this resource includes the segment that the campaign reaches out to, the message that it delivers, and the schedule on which it runs. You can use this resource to look up, create, update, or delete campaigns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a310cb5a-6e74-4ddd-b147-e5831873be9f"
            }
          ]
        }
      ]
    }
  ]
}