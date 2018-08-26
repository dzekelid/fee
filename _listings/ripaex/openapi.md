---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
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
  /api/blocks/getFee:
    get:
      summary: Blocks Get Fee
      description: Get the transaction fee for sending "normal" transactions.
      operationId: blocks.getFee
      x-api-path-slug: apiblocksgetfee-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fee
  /api/delegates/fee:
    get:
      summary: Delegates Fee
      description: Get the delegate fee.
      operationId: delegates.getFee
      x-api-path-slug: apidelegatesfee-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Fee
  /api/signatures/fee:
    get:
      summary: Signatures Fee
      description: Get the fee for a signature.
      operationId: signatures.fee
      x-api-path-slug: apisignaturesfee-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Signatures
      - Fee
  /api/blocks/getFees:
    get:
      summary: Blocks Get Fees
      description: Get the network fees.
      operationId: blocks.getFees
      x-api-path-slug: apiblocksgetfees-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fees
---