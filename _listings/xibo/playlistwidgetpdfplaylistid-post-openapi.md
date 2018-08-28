---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Parameters for editing existing pdf on a layout
  description: Parameters for editing existing pdf on a layout, for adding new files,
    please refer to POST /library documentation
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/pdf/{playlistId}:
    post:
      summary: Parameters for editing existing pdf on a layout
      description: Parameters for editing existing pdf on a layout, for adding new
        files, please refer to POST /library documentation
      operationId: WidgetPdfEdit
      x-api-path-slug: playlistwidgetpdfplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: name
        description: Edit only - Optional Widget Name
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Pdf
      - "On"
      - Layout
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