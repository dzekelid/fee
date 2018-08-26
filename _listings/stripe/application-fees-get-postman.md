{
  "info": {
    "name": "Stripe Get Application Fees",
    "_postman_id": "2d7653a0-d082-46eb-9c53-201b4d7532c5",
    "description": "Returns a list of application fees you???ve previously collected. The application fees are returned in sorted order, with the most recent fees appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "application",
      "item": [
        {
          "id": "8d7d8732-8d76-4cb0-a2d6-31a1ef484977",
          "name": "getApplicationFees",
          "request": {
            "url": "http://api.stripe.com/v1/application_fees?charge=%7B%7D&created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of application fees you???ve previously collected"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f423dcc8-bd87-4db4-961b-666401a2dd19"
            }
          ]
        }
      ]
    }
  ]
}