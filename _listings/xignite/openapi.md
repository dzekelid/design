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
  ', Design':
    get:
      summary: Get Chart Design
      description: Returns the default design class for the statistics Chart.
      operationId: postGetchartdesign
      x-api-path-slug: design-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Design
  Intraday, , Design:
    get:
      summary: Get Intraday Chart Design
      description: Returns the default settings for the intraday future chart.
      operationId: postGetintradaychartdesign
      x-api-path-slug: intraday--design-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Intraday
      - Chart
      - Design
  Historical, , Design:
    get:
      summary: Get Historical Chart Design
      description: Returns the default settings for the historical future chart.
      operationId: postGethistoricalchartdesign
      x-api-path-slug: historical--design-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Chart
      - Design