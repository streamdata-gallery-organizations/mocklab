---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Put Mappings Stubmappingid
  version: 1.0.0
  description: Update an existing stub mapping
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mappings:
    delete:
      summary: Delete Mappings
      description: Delete all stub mappings
      operationId: deleteMappings
      x-api-path-slug: mappings-delete
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
    get:
      summary: Get Mappings
      description: Get all stub mappings
      operationId: getMappings
      x-api-path-slug: mappings-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: The start index of the results to return
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
    post:
      summary: Post Mappings
      description: Create a new stub mapping
      operationId: postMappings
      x-api-path-slug: mappings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
  /mappings/find-by-metadata:
    post:
      summary: Post Mappings Find By Metadata
      description: Find stubs by matching on their metadata
      operationId: postMappingsFindByMetadata
      x-api-path-slug: mappingsfindbymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Find
      - Metadata
  /mappings/remove-by-metadata:
    post:
      summary: Post Mappings Remove By Metadata
      description: Remove stubs by matching on their metadata
      operationId: postMappingsRemoveByMetadata
      x-api-path-slug: mappingsremovebymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Remove
      - Metadata
  /mappings/reset:
    post:
      summary: Post Mappings Reset
      description: Reset stub mappings (restore to defaults defined back the backing
        store)
      operationId: postMappingsReset
      x-api-path-slug: mappingsreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Reset
  /mappings/save:
    post:
      summary: Post Mappings Save
      description: Save all persistent stub mappings to the backing store
      operationId: postMappingsSave
      x-api-path-slug: mappingssave-post
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Save
  /mappings/{stubMappingId}:
    delete:
      summary: Delete Mappings Stubmappingid
      description: Delete mappings stubmappingid.
      operationId: deleteMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-delete
      parameters:
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
    get:
      summary: Get Mappings Stubmappingid
      description: Get mappings stubmappingid.
      operationId: getMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-get
      parameters:
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
    put:
      summary: Put Mappings Stubmappingid
      description: Update an existing stub mapping
      operationId: putMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
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