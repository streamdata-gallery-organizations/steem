---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem Account
  description: Get Accounts from Steem
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
  /get_witness_schedule:
    get:
      summary: get_witness_schedule
      description: get_witness_schedule
      operationId: get-witness-schedule
      x-api-path-slug: get-witness-schedule-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Schedule
  /get_witnesses:
    get:
      summary: get_witnesses
      description: get_witnesses
      operationId: get-witnesses
      x-api-path-slug: get-witnesses-get
      parameters:
      - in: query
        name: witnessIds
        description: witnessIds
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witnesses
  /get_witness_by_account:
    get:
      summary: get_witness_by_account
      description: get_witness_by_account
      operationId: get-witness-by-account
      x-api-path-slug: get-witness-by-account-get
      parameters:
      - in: query
        name: accountName
        description: witness account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - By
      - Account
  /get_witnesses_by_vote:
    get:
      summary: get_witnesses_by_vote
      description: get_witnesses_by_vote
      operationId: get-witnesses-by-vote
      x-api-path-slug: get-witnesses-by-vote-get
      parameters:
      - in: query
        name: from
        description: from witness
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witnesses
      - By
      - Vote
  /get_active_witnesses:
    get:
      summary: get_active_witnesses
      description: get_active_witnesses
      operationId: get-active-witnesses
      x-api-path-slug: get-active-witnesses-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Active
      - Witnesses
  /witness_update:
    get:
      summary: witness_update
      description: witness_update
      operationId: witness-update
      x-api-path-slug: witness-update-get
      parameters:
      - in: query
        name: block_signing_key
        description: block_signing_key
      - in: query
        name: fee
        description: fee
      - in: query
        name: owner
        description: witness name
      - in: query
        name: props
        description: props
      - in: query
        name: url
        description: url
      responses:
        200:
          description: OK
      tags:
      - Witness
      - Update
  /get_miner_queue:
    get:
      summary: get_miner_queue
      description: get_miner_queue
      operationId: get-miner-queue
      x-api-path-slug: get-miner-queue-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Miner
      - Queue
  /get_liquidity_queue:
    get:
      summary: get_liquidity_queue
      description: get_liquidity_queue
      operationId: get-liquidity-queue
      x-api-path-slug: get-liquidity-queue-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: startAccount
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Liquidity
      - Queue
  /get_open_orders:
    get:
      summary: get_open_orders
      description: get_open_orders
      operationId: get-open-orders
      x-api-path-slug: get-open-orders-get
      parameters:
      - in: query
        name: owner
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Open
      - Orders
  /get_order_book:
    get:
      summary: get_order_book
      description: get_order_book
      operationId: get-order-book
      x-api-path-slug: get-order-book-get
      parameters:
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Order
      - Book
  /get_active_categories:
    get:
      summary: get active categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-active-categories-get
      parameters:
      - in: query
        name: after
        description: after string
      - in: query
        name: limit
        description: limit size
      responses:
        200:
          description: OK
      tags:
      - Get
      - Active
      - Categories
  /get_best_categories:
    get:
      summary: get best categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-best-categories-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: limit
        description: limits
      responses:
        200:
          description: OK
      tags:
      - Get
      - Best
      - Categories
  /get_recent_categories:
    get:
      summary: get recent categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-recent-categories-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Recent
      - Categories
  /get_trending_categories:
    get:
      summary: get trending categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-trending-categories-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: limit
        description: limits
      responses:
        200:
          description: OK
      tags:
      - Get
      - Trending
      - Categories
  /get_trending_tags:
    get:
      summary: get trending categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-trending-tags-get
      parameters:
      - in: query
        name: afterTag
        description: category
      - in: query
        name: limit
        description: limits
      responses:
        200:
          description: OK
      tags:
      - Get
      - Trending
      - Categories
  /get_content:
    get:
      summary: get content
      description: get content
      operationId: get-content
      x-api-path-slug: get-content-get
      parameters:
      - in: query
        name: author
        description: author
      - in: query
        name: permlink
        description: permlink
      responses:
        200:
          description: OK
      tags:
      - Get
      - Content
  /get_content_replies:
    get:
      summary: get content replies
      description: get content replies
      operationId: get-content-replies
      x-api-path-slug: get-content-replies-get
      parameters:
      - in: query
        name: author
        description: author
      - in: query
        name: permlink
        description: permlink
      responses:
        200:
          description: OK
      tags:
      - Get
      - Content
      - Replies
  /get_discussions_by_trending:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-trending-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_trending30:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-trending30-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_created:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-created-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_active:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-active-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_promoted:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-promoted-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_cashout:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-cashout-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_payout:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-payout-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_votes:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-votes-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_children:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-children-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_hot:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"steem"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsteem-or-start-authorauthor-permlinkpermlink-for-paginatio
      x-api-path-slug: get-discussions-by-hot-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_feed:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tags":"good-karma"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-tagsgoodkarma-or-start-authorauthor-permlinkpermlink-for-pagi
      x-api-path-slug: get-discussions-by-feed-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_blog:
    get:
      summary: get discussions
      description: get discussions, | query example {"limit":"10", "tag":"good-karma"}
        OR {"start_author":"author", "permlink":"permlink"} for pagination
      operationId: get-discussions--query-example-limit10-taggoodkarma-or-start-authorauthor-permlinkpermlink-for-pagin
      x-api-path-slug: get-discussions-by-blog-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_comments:
    get:
      summary: get discussions
      description: get discussions, | query example {"start_author":"author", "start_permlink":"permlink",
        "limi":"10"}
      operationId: get-discussions--query-example-start-authorauthor-start-permlinkpermlink-limi10
      x-api-path-slug: get-discussions-by-comments-get
      parameters:
      - in: query
        name: query
        description: query object
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
  /get_discussions_by_author_before_date:
    get:
      summary: get_discussions_by_author_before_date
      description: get_discussions_by_author_before_date
      operationId: get-discussions-by-author-before-date
      x-api-path-slug: get-discussions-by-author-before-date-get
      parameters:
      - in: query
        name: author
        description: account name
      - in: query
        name: beforeDate
        description: date and time
      - in: query
        name: limit
        description: limit query
      - in: query
        name: startPermlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Discussions
      - By
      - Author
      - Before
      - Date
  /get_replies_by_last_update:
    get:
      summary: get_replies_by_last_update
      description: get_replies_by_last_update
      operationId: get-replies-by-last-update
      x-api-path-slug: get-replies-by-last-update-get
      parameters:
      - in: query
        name: limit
        description: limit query
      - in: query
        name: startAuthor
        description: account name
      - in: query
        name: startPermlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Replies
      - By
      - Last
      - Update
  /get_state:
    get:
      summary: get_state
      description: get_state
      operationId: get-state
      x-api-path-slug: get-state-get
      parameters:
      - in: query
        name: path
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - State
  /get_active_votes:
    get:
      summary: get_active_votes
      description: get_active_votes
      operationId: get-active-votes
      x-api-path-slug: get-active-votes-get
      parameters:
      - in: query
        name: author
        description: account name
      - in: query
        name: permlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Active
      - Votes
  /get_account_votes:
    get:
      summary: get_account_votes
      description: get_account_votes
      operationId: get-account-votes
      x-api-path-slug: get-account-votes-get
      parameters:
      - in: query
        name: voter
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Votes
  /get_account_history:
    get:
      summary: Account history
      description: Account history
      operationId: account-history
      x-api-path-slug: get-account-history-get
      parameters:
      - in: query
        name: account
        description: name of account
      - in: query
        name: from
        description: from
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Account
      - History
  /get_owner_history:
    get:
      summary: get_owner_history
      description: get_owner_history
      operationId: get-owner-history
      x-api-path-slug: get-owner-history-get
      parameters:
      - in: query
        name: account
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Owner
      - History
  /get_accounts:
    get:
      summary: Account
      description: Get Accounts from Steem
      operationId: get-accounts-from-steem
      x-api-path-slug: get-accounts-get
      parameters:
      - in: query
        name: names[]
        description: name of account
      responses:
        200:
          description: OK
      tags:
      - Account
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