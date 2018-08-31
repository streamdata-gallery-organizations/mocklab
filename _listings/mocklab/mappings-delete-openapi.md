---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Delete Mappings
  version: 1.0.0
  description: Delete all stub mappings
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