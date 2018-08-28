---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Accounts Delegates Fee
  description: Get the delegate fee of an account.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/delegates/fee:
    get:
      summary: Accounts Delegates Fee
      description: Get the delegate fee of an account.
      operationId: accounts.getDelegatesFee
      x-api-path-slug: apiaccountsdelegatesfee-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Delegates
      - Fee
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