---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get chain properties
  description: get chain properties
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_version:
    get:
      summary: get version of Steem
      description: Returns version information of connected Steem node/websocket.
      operationId: returns-version-information-of-connected-steem-nodewebsocket
      x-api-path-slug: get-version-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Version
      - Of
      - Steem
  /get_account_count:
    get:
      summary: number of accounts
      description: Get Number of Accounts from Steem
      operationId: get-number-of-accounts-from-steem
      x-api-path-slug: get-account-count-get
      responses:
        200:
          description: OK
      tags:
      - Number
      - Of
      - Accounts
  /get_chain_properties:
    get:
      summary: get chain properties
      description: get chain properties
      operationId: get-chain-properties
      x-api-path-slug: get-chain-properties-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Chain
      - Properties
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