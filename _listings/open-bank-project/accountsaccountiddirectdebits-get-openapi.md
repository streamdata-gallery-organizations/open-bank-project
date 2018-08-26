---
swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 0
info:
  title: Open Bank Project Get Account Direct Debits
  description: Get Direct Debits related to an account
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account-requests:
    post:
      summary: Create an account request
      description: Create an account request
      operationId: CreateAccountRequest
      x-api-path-slug: accountrequests-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Request
  /account-requests/{AccountRequestId}:
    get:
      summary: Get an account request
      description: Get an account request
      operationId: GetAccountRequest
      x-api-path-slug: accountrequestsaccountrequestid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Request
    delete:
      summary: Delete an account request
      description: Delete an account request
      operationId: DeleteAccountRequest
      x-api-path-slug: accountrequestsaccountrequestid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Request
  /accounts:
    get:
      summary: Get Accounts
      description: Get a list of accounts
      operationId: GetAccounts
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Accounts
  /accounts/{AccountId}:
    get:
      summary: Get Account
      description: Get an account
      operationId: GetAccount
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
  /accounts/{AccountId}/transactions:
    get:
      summary: Get Account Transactions
      description: Get transactions related to an account
      operationId: GetAccountTransactions
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Transactions
  /accounts/{AccountId}/beneficiaries:
    get:
      summary: Get Account Beneficiaries
      description: Get Beneficiaries related to an account
      operationId: GetAccountBeneficiaries
      x-api-path-slug: accountsaccountidbeneficiaries-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Beneficiaries
  /accounts/{AccountId}/balances:
    get:
      summary: Get Account Balances
      description: Get Balances related to an account
      operationId: GetAccountBalances
      x-api-path-slug: accountsaccountidbalances-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Balances
  /accounts/{AccountId}/direct-debits:
    get:
      summary: Get Account Direct Debits
      description: Get Direct Debits related to an account
      operationId: GetAccountDirectDebits
      x-api-path-slug: accountsaccountiddirectdebits-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Direct
      - Debits
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