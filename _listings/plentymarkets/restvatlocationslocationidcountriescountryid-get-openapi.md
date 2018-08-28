---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List VAT configurations for one country of delivery
  description: Lists the VAT configurations for a country of delivery of one accounting
    location. The ID of the accounting location and the ID of the country of delivery
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/vat/locations/{locationId}/countries/{countryId}:
    get:
      summary: List VAT configurations for one country of delivery
      description: Lists the VAT configurations for a country of delivery of one accounting
        location. The ID of the accounting location and the ID of the country of delivery
        must be specified.
      operationId: getRestVatLocationsLocationCountriesCountry
      x-api-path-slug: restvatlocationslocationidcountriescountryid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurationsone
      - Country
      - Of
      - Delivery
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