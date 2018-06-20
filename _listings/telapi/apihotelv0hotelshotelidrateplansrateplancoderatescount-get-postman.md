{
  "info": {
    "name": "hetras Hotel API Version 0 Get the count of all active and loaded daily rates for the defined rateplan in a specified time period.",
    "_postman_id": "07eb09b4-318a-49d7-90a1-7fcdc6eab534",
    "description": "Get the count of all active and loaded daily rates for the defined rateplan in a specified time period..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Count",
      "item": [
        {
          "id": "c26d9ae0-a4a1-4097-8c92-896d2155b267",
          "name": "RatePlans_GetRatesCount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rateplans/:rateplanCode/rates/$count"
              ],
              "query": [
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "hotelId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "rateplanCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "App-Id",
                "value": "{}",
                "description": "Application identifier",
                "disabled": false
              },
              {
                "key": "App-Key",
                "value": "{}",
                "description": "Application key",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the count of all active and loaded daily rates for the defined rateplan in a specified time period.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d0010a4-7ecb-421b-8307-11bedc447334"
            }
          ]
        }
      ]
    }
  ]
}