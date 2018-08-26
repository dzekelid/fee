---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 1
info:
  title: Expedia
  description: expedia-mobile-api-documentation--brfont-colorblue-note-in-case-of-authorization-exception-just-a-hrefstaticmobileswaggeruiusersigninusersigninafont
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/flight/trip/cardFee:
    post:
      summary: Get the credit card fee for a trip
      description: This api provides an accurate credit card fee that a user would
        have to pay when booking a trip.
      operationId: flights-trip-fee
      x-api-path-slug: apiflighttripcardfee-post
      parameters:
      - in: formData
        name: clientId
        description: Client Id
      - in: formData
        name: creditCardId
        description: This is a string that identifies the credit card that will be
          used to pay for the trip
      - in: formData
        name: tripId
        description: The id of the trip to get the credit card fee for
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Airports
      - Airplanes
      - Airlines
---