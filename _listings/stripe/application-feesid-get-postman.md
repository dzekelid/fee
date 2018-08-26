{
  "info": {
    "name": "Stripe Get Application Fees",
    "_postman_id": "6573cb6a-d55c-4fd9-8677-626f27fcc3b8",
    "description": "Retrieves the details of an application fee that your account has collected. The same information is returned when refunding the application fee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "application",
      "item": [
        {
          "id": "5f5447f3-e549-4b12-8e46-e30a79e49177",
          "name": "getApplicationFees",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "application_fees/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details of an application fee that your account has collected"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "674108d2-ba24-4af7-9b58-0b08d3857617"
            }
          ]
        }
      ]
    }
  ]
}