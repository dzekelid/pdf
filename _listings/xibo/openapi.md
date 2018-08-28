swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
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