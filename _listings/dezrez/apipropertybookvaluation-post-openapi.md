---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez A command driven endpoint to Book a Valuation.
  version: 1.0.0
  description: A command driven endpoint to book a valuation..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/bookvaluation:
    post:
      summary: A command driven endpoint to Book a Valuation.
      description: A command driven endpoint to book a valuation..
      operationId: Property_BookValuationBybookValuationData
      x-api-path-slug: apipropertybookvaluation-post
      parameters:
      - in: body
        name: bookValuationData
        description: A wrapper for the various data contracts needed
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - Book
      - Valuation
  /api/property/recordvaluation:
    post:
      summary: A command driven endpoint to Record a Valuation.
      description: A command driven endpoint to record a valuation..
      operationId: Property_RecordValuationByrecordValuationData
      x-api-path-slug: apipropertyrecordvaluation-post
      parameters:
      - in: body
        name: recordValuationData
        description: A wrapper for the various data contracts needed
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - Record
      - Valuation
  /api/property/{id}/updateaddress:
    put:
      summary: A command driven endpoint to Update a property address.
      description: A command driven endpoint to update a property address..
      operationId: Property_UpdateAddressByidByaddressDataContract
      x-api-path-slug: apipropertyidupdateaddress-put
      parameters:
      - in: body
        name: addressDataContract
        description: The address data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - ""
      - Property
      - Address
  /api/property/updatevaluation:
    put:
      summary: A command driven endpoint to Update a Valuation.
      description: A command driven endpoint to update a valuation..
      operationId: Property_UpdateValuationByvaluationDataContract
      x-api-path-slug: apipropertyupdatevaluation-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: valuationDataContract
        description: The valuation data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - ""
      - Valuation
  /api/people/updatepeople:
    put:
      summary: Update a Person's detailsCommand
      description: Update a person's detailscommand.
      operationId: People_UpdatePeopleBypeopleCommandDataContract
      x-api-path-slug: apipeopleupdatepeople-put
      parameters:
      - in: body
        name: peopleCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Persons
      - DetailsCommand
  /api/people/updateperson:
    put:
      summary: Update a Person's detailsCommand
      description: Update a person's detailscommand.
      operationId: People_UpdatePersonBypersonCommandDataContract
      x-api-path-slug: apipeopleupdateperson-put
      parameters:
      - in: body
        name: personCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Persons
      - DetailsCommand
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