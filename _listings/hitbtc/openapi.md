---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trading/fee/{symbol}:
    get:
      summary: Get Trading Fee Rate
      description: Get trading fee rate.
      operationId: getTradingFeeSymbol
      x-api-path-slug: tradingfeesymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Trading
      - Fee
      - Rate
---