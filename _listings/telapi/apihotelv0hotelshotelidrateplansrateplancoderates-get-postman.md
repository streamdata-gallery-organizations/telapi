{
  "info": {
    "name": "hetras Hotel API Version 0 Get the setup of the daily rates for a specific rateplan and a defined timeperiod.",
    "_postman_id": "d7e35cc1-bd21-42f2-b674-248b9ec4bfb5",
    "description": "With this call you can read the daily rates setup including the cancellation policy and minimum guarantee per day for the\r\n            specified rateplan. You can specify a timeperiod to read the daily rates for. The rateplan needs to be active for at least\r\n            one business day in the defined time period and have rates loaded.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Setup",
      "item": [
        {
          "id": "7d7f0909-228d-44e3-8cbd-9eba4ebcb7af",
          "name": "RatePlans_GetRates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rateplans/:rateplanCode/rates"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "inlinecount",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "top",
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
            "description": "With this call you can read the daily rates setup including the cancellation policy and minimum guarantee per day for the\r\n            specified rateplan. You can specify a timeperiod to read the daily rates for. The rateplan needs to be active for at least\r\n            one business day in the defined time period and have rates loaded."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "848bd07d-c098-446d-9a87-86b7d8ddd59a"
            }
          ]
        }
      ]
    }
  ]
}