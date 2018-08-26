---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Healthcheck for custom datasource.
  version: 1.0.0
  description: Indicates whether custom data connector is up and running.
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