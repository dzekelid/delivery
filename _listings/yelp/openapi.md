swagger: "2.0"
x-collection-name: Yelp
x-complete: 1
info:
  title: Yelp V3
  description: yelps-fusion-api-allows-you-to-get-the-best-local-business-information-and-user-reviews-of-over-million-businesses-in-32-countries
  version: 1.0.0
host: api.yelp.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions/delivery/search:
    get:
      summary: Get Transactions Delivery Search
      description: Get transactions delivery search.
      operationId: getTransactionsDeliverySearch
      x-api-path-slug: transactionsdeliverysearch-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Delivery
      - Search