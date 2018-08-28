---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Write analytic output data to custom datasource.
  version: 1.0.0
  description: Writes analytic output data generated during runtime execution.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/analytics/customdata/healthcheck:
    get:
      summary: Healthcheck for custom datasource.
      description: Indicates whether custom data connector is up and running.
      operationId: healthcheck
      x-api-path-slug: apiv1analyticscustomdatahealthcheck-get
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Healthcheckcustom
      - Datasource
  /api/v1/analytics/customdata/read:
    post:
      summary: Retrieve analytic input data from custom datasource.
      description: Returns the analytic input data used during runtime execution.
      operationId: readCustomProviderData
      x-api-path-slug: apiv1analyticscustomdataread-post
      parameters:
      - in: body
        name: body
        description: Analytic Input Data Read request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Analytic
      - Input
      - Data
      - From
      - Custom
      - Datasource
  /api/v1/analytics/customdata/write:
    post:
      summary: Write analytic output data to custom datasource.
      description: Writes analytic output data generated during runtime execution.
      operationId: writeCustomProviderData
      x-api-path-slug: apiv1analyticscustomdatawrite-post
      parameters:
      - in: body
        name: body
        description: Analytic Output Data Write Request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Write
      - Analytic
      - Output
      - Data
      - To
      - Custom
      - Datasource
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