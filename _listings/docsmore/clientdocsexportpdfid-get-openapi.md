---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Export As PDF
  description: In order to export as PDf, you will need to have client document ID
    available for that specific document you are looking to download.
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clientdocs/exportpdf/{id}:
    get:
      summary: Export As PDF
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: ClientdocsExportpdfByIdGet
      x-api-path-slug: clientdocsexportpdfid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Export
      - As
      - PDF
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