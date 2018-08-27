{
  "info": {
    "name": "Constant Contact Get Per-Contact Campaign Events",
    "_postman_id": "3420e4a1-175d-4458-8a3c-43a17c8b96dc",
    "description": "Get Per-Contact Campaign Events",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaign",
      "item": [
        {
          "id": "7ad7bad2-8436-4661-8270-041e0a21137a",
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
              "id": "38d09808-aa4c-406d-a8d7-4b7da3b1a308"
            }
          ]
        }
      ]
    },
    {
      "name": "Per-Contact",
      "item": [
        {
          "id": "c1e1f0bb-7719-4364-b154-a30e5e3cf252",
          "name": "get-percontact-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id/events/"
              ],
              "variable": [
                {
                  "id": "contact-id",
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
            "description": "Get Per-Contact Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d0a4d89-6c33-4ef6-863e-4fa184a3c8b8"
            }
          ]
        }
      ]
    }
  ]
}