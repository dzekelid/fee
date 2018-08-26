---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/fees:
    post:
      summary: Creates a fee (tax).
      description: Creates a fee (tax).
      operationId: CreateFee
      x-api-path-slug: v1location-idfees-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a fee for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Fee
      - (tax)
  /v1/{location_id}/fees/{fee_id}:
    delete:
      summary: Deletes an existing fee (tax).
      description: Deletes an existing fee (tax).
      operationId: DeleteFee
      x-api-path-slug: v1location-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to delete
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Fee
      - (tax)
    put:
      summary: Modifies the details of an existing fee (tax).
      description: Modifies the details of an existing fee (tax).
      operationId: UpdateFee
      x-api-path-slug: v1location-idfeesfee-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fee_id
        description: The ID of the fee to edit
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Fee
      - (tax)
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
    put:
      summary: Associates a fee with an item, meaning the fee is automatically applied
        to the item in Square Register.
      description: Associates a fee with an item, meaning the fee is automatically
        applied to the item in Square Register.
      operationId: ApplyFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-put
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Fee
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
---