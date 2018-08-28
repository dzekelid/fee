---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Pricing Fee Rates
  description: |-
    Returns a list of fee_rate objects for the different
    currencies, countries, assortments and sales channels we sell through
    today and in the future.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pricing/fee_rates/:
    get:
      summary: Get Pricing Fee Rates
      description: |-
        Returns a list of fee_rate objects for the different
        currencies, countries, assortments and sales channels we sell through
        today and in the future.
      operationId: getPricingFeeRates
      x-api-path-slug: pricingfee-rates-get
      parameters:
      - in: query
        name: channel
        description: The sales channel
        type: query
      - in: query
        name: country
        description: The (ISO 3166 alpha-2 code of the) country where you want to
          know the fee rates
        type: query
      - in: query
        name: currency
        description: The (ISO 4217 3-character code of the) currency where you want
          to know the fee rates
        type: query
      - in: query
        name: item_type
        description: The item type for which get the price fee rates
        type: query
      - in: query
        name: payment_type
        description: The payment type to get the price for
        type: query
      - in: query
        name: plan
        description: The assortment package name to get the price for
        type: query
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Fee
      - Rates
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