swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/createpdf:
    post:
      summary: Creates a new pdf document.
      description: Creates a new pdf document..
      operationId: DocumentGeneration_CreatePdfBypdfData
      x-api-path-slug: apidocumentgenerationcreatepdf-post
      parameters:
      - in: body
        name: pdfData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Pdf
      - Document