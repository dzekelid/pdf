---
swagger: "2.0"
x-collection-name: ConvertAPI
x-complete: 0
info:
  title: Convert API PDF to PDF
  description: The API for converting PDF documents to Image. These file formats pdf
    can be converted to pdf, pdfa, png, jpg, tif.
  version: v1
host: do.convertapi.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Email2Pdf:
    post:
      summary: Email to PDF
      description: The API for converting E-Mail files to PDF files and Images. These
        file formats eml, mbx, msg, oft can be converted to pdf, pdfa, png, jpg, tif.
      operationId: email2pdf
      x-api-path-slug: email2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: eml, mbx, msg, oft'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Email
      - PDF
  /Excel2Pdf:
    post:
      summary: Excel to PDF
      description: The API for converting Excel documents to PDF files and Images.
        These file formats csv, xls, xlsb, xlsx, xlt, xltx can be converted to pdf,
        pdfa, png, jpg, tif.
      operationId: excel2pdf
      x-api-path-slug: excel2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: csv, xls, xlsb, xlsx, xlt, xltx'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: WorksheetActive
        description: Set to convert active worksheet
      - in: query
        name: WorksheetIndex
        description: Set worksheet index(number) to convert
      - in: query
        name: WorksheetName
        description: Set worksheet name to convert
      responses:
        200:
          description: OK
      tags:
      - Excel
      - PDF
  /Image2Pdf:
    post:
      summary: Image to PDF
      description: The API for converting Image files to PDF files and Images. These
        file formats avs, bmp, dcx, dib, dpx, fax, fits, fpx, gif, ico, iptc, jbig,
        jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv, otb, pbm, pcd, pcds, pct, pcx, pgm,
        pict, png, pnm, ppm, psd, p7, ras, rgba, sun, tga, tiff, tif, vicar, vid,
        viff, wmf, xbm, xpm, xwd can be converted to pdf, pdfa, png, jpg, tif.
      operationId: image2pdf
      x-api-path-slug: image2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: avs, bmp, dcx, dib, dpx, fax,
          fits, fpx, gif, ico, iptc, jbig, jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv,
          otb, pbm, pcd, pcds, pct, pcx, pgm, pict, png, pnm, ppm, psd, p7, ras, rgba,
          sun, tga, tiff, tif, vicar, vid, viff, wmf, xbm, xpm, xwd'
      - in: query
        name: Ocr
        description: Apply optical character recognition (OCR) and convert scanned
          text images into editable and searchable PDF
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Image
      - PDF
  /Journal2Pdf:
    post:
      summary: Journal to PDF
      description: The API for converting Windows Journal Viewer documents to PDF
        files and Images. These file formats jnt can be converted to pdf, pdfa, png,
        jpg, tif.
      operationId: journal2pdf
      x-api-path-slug: journal2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: jnt'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Journal
      - PDF
  /Lotus2Pdf:
    post:
      summary: Lotus to PDF
      description: The API for converting Lotus Smart Suite documents to PDF files
        and Images. These file formats 123, 12m, wk1, wk2, wk3, lwp, mwp, sam can
        be converted to pdf, pdfa, png, jpg, tif.
      operationId: lotus2pdf
      x-api-path-slug: lotus2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: 123, 12m, wk1, wk2, wk3, lwp,
          mwp, sam'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Lotus
      - PDF
  /OpenOffice2Pdf:
    post:
      summary: Open Office to PDF
      description: The API for converting OpenOffice documents to PDF files and Images.
        These file formats mml, odc, odf, odg, odi, odm, odp, ods, odt, otg, oth,
        otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc, sxg, sxi, sxm, sxw, vor,
        wv2 can be converted to pdf, pdfa, png, jpg, tif.
      operationId: openoffice2pdf
      x-api-path-slug: openoffice2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: mml, odc, odf, odg, odi, odm,
          odp, ods, odt, otg, oth, otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc,
          sxg, sxi, sxm, sxw, vor, wv2'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Open
      - Office
      - PDF
  /Pdf2Image:
    post:
      summary: PDF to Image
      description: The API for converting PDF documents to Image. These file formats
        pdf can be converted to png, jpg, tif.
      operationId: pdf2image
      x-api-path-slug: pdf2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: pdf'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - PDF
      - Image
  /Pdf2Pdf:
    post:
      summary: PDF to PDF
      description: The API for converting PDF documents to Image. These file formats
        pdf can be converted to pdf, pdfa, png, jpg, tif.
      operationId: pdf2pdf
      x-api-path-slug: pdf2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: pdf'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - PDF
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