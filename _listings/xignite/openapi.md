swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLogosList:
    get:
      summary: Get Logos List
      description: Get all symbols which have available logos.
      operationId: postGetlogoslist
      x-api-path-slug: getlogoslist-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Logos
      - List
  /GetLogo:
    get:
      summary: Get Logo
      description: Save an archive.
      operationId: postGetlogo
      x-api-path-slug: getlogo-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Logo