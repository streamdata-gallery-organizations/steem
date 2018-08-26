---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem lookup_witness_accounts
  description: lookup_witness_accounts regex search
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
  /get_config:
    get:
      summary: get config
      description: get config
      operationId: get-config
      x-api-path-slug: get-config-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Config
  /get_dynamic_global_properties:
    get:
      summary: get_dynamic_global_properties
      description: get_dynamic_global_properties
      operationId: get-dynamic-global-properties
      x-api-path-slug: get-dynamic-global-properties-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Dynamic
      - Global
      - Properties
  /get_feed_history:
    get:
      summary: get_feed_history
      description: get_feed_history
      operationId: get-feed-history
      x-api-path-slug: get-feed-history-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Feed
      - History
  /get_current_median_history_price:
    get:
      summary: get_current_median_history_price
      description: get_current_median_history_price
      operationId: get-current-median-history-price
      x-api-path-slug: get-current-median-history-price-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Current
      - Median
      - History
      - Price
  /get_hardfork_version:
    get:
      summary: get_hardfork_version
      description: get_hardfork_version
      operationId: get-hardfork-version
      x-api-path-slug: get-hardfork-version-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Hardfork
      - Version
  /get_next_scheduled_hardfork:
    get:
      summary: get_next_scheduled_hardfork
      description: get_next_scheduled_hardfork
      operationId: get-next-scheduled-hardfork
      x-api-path-slug: get-next-scheduled-hardfork-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Next
      - Scheduled
      - Hardfork
  /get_witness_count:
    get:
      summary: get_witness_count
      description: get_witness_count
      operationId: get-witness-count
      x-api-path-slug: get-witness-count-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Count
  /lookup_witness_accounts:
    get:
      summary: lookup_witness_accounts
      description: lookup_witness_accounts regex search
      operationId: lookup-witness-accounts-regex-search
      x-api-path-slug: lookup-witness-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Witness
      - Accounts
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