{
  "info": {
    "name": "Stripe Get Application Fees Fee Refunds",
    "_postman_id": "d0aa5b1c-0d78-4906-a647-9b46f6326255",
    "description": "By default, you can see the 10 most recent refunds stored directly on the application fee object, but you can also retrieve details about a specific refund stored on the application fee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "application",
      "item": [
        {
          "id": "2d1a3f99-1b6f-49da-887b-c3d5ee0df0fa",
          "name": "getApplicationFeesFeeRefunds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "application_fees/:fee/refunds/:id"
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
                  "id": "fee",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "By default, you can see the 10 most recent refunds stored directly on the application fee object, but you can also retrieve details about a specific refund stored on the application fee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68364575-56f5-486f-a298-1f57e603a950"
            }
          ]
        }
      ]
    }
  ]
}