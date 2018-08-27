{
  "info": {
    "name": "Constant Contact Get Campaign Events",
    "_postman_id": "caade5da-2ef6-42a6-b8c4-5ad2aef8acd2",
    "description": "Get Campaign Events",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaign",
      "item": [
        {
          "id": "ac087bcc-e5f7-49ee-9d9c-8c7f2bdadc91",
          "name": "get-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id/events/"
              ],
              "variable": [
                {
                  "id": "campaign-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7588b9a-003a-4f60-8514-6c08d5066287"
            }
          ]
        }
      ]
    }
  ]
}