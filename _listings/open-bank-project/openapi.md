---
swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
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
  /accounts/{AccountId}/standing-orders:
    get:
      summary: Get Account Standing Orders
      description: Get Standing Orders related to an account
      operationId: GetAccountStandingOrders
      x-api-path-slug: accountsaccountidstandingorders-get
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
      - Standing
      - Orders
  /accounts/{AccountId}/product:
    get:
      summary: Get Account Product
      description: Get Product related to an account
      operationId: GetAccountProduct
      x-api-path-slug: accountsaccountidproduct-get
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
      - Product
  /accounts/{AccountId}/offers:
    get:
      summary: Get Account Offers
      description: Get Offers related to an account
      operationId: GetAccountOffers
      x-api-path-slug: accountsaccountidoffers-get
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
      - Offers
  /accounts/{AccountId}/party:
    get:
      summary: Get Account Party
      description: Get Party related to an account
      operationId: GetAccountParty
      x-api-path-slug: accountsaccountidparty-get
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
      - Party
  /accounts/{AccountId}/scheduled-payments:
    get:
      summary: Get Account Scheduled Payments
      description: Get Scheduled Payments related to an account
      operationId: GetAccountScheduledPayments
      x-api-path-slug: accountsaccountidscheduledpayments-get
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
      - Scheduled
      - Payments
  /accounts/{AccountId}/statements:
    get:
      summary: Get Account Statements
      description: Get Statements related to an account
      operationId: GetAccountStatements
      x-api-path-slug: accountsaccountidstatements-get
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
      - Statements
  /accounts/{AccountId}/statements/{StatementId}:
    get:
      summary: Get Statement
      description: Get Statement related to an account
      operationId: GetAccountStatement
      x-api-path-slug: accountsaccountidstatementsstatementid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
  /accounts/{AccountId}/statements/{StatementId}/file:
    get:
      summary: Get Statement File
      description: Get Statement File related to an account
      operationId: GetAccountStatementFile
      x-api-path-slug: accountsaccountidstatementsstatementidfile-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
      - File
  /accounts/{AccountId}/statements/{StatementId}/transactions:
    get:
      summary: Get Statement Transactions
      description: Get Statement Transactions related to an account
      operationId: GetAccountStatementTransactions
      x-api-path-slug: accountsaccountidstatementsstatementidtransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
      - Transactions
  /standing-orders:
    get:
      summary: Get Standing Orders
      description: Get Standing Orders
      operationId: GetStandingOrders
      x-api-path-slug: standingorders-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Standing
      - Orders
  /direct-debits:
    get:
      summary: Get Direct Debits
      description: Get Direct Debits
      operationId: GetDirectDebits
      x-api-path-slug: directdebits-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Direct
      - Debits
  /beneficiaries:
    get:
      summary: Get Beneficiaries
      description: Get Beneficiaries
      operationId: GetBeneficiaries
      x-api-path-slug: beneficiaries-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Beneficiaries
  /transactions:
    get:
      summary: Get Transactions
      description: Get Transactions
      operationId: GetTransactions
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Transactions
  /balances:
    get:
      summary: Get Balances
      description: Get Balances
      operationId: GetBalances
      x-api-path-slug: balances-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Balances
  /products:
    get:
      summary: Get Products
      description: Get Products
      operationId: GetProducts
      x-api-path-slug: products-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Products
  /offers:
    get:
      summary: Get Offers
      description: Get Offers
      operationId: GetOffers
      x-api-path-slug: offers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Offers
  /party:
    get:
      summary: Get Party
      description: Get Party
      operationId: GetParty
      x-api-path-slug: party-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Party
  /scheduled-payments:
    get:
      summary: Get Scheduled Payments
      description: Get Scheduled Payments
      operationId: GetScheduledPayments
      x-api-path-slug: scheduledpayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Scheduled
      - Payments
  /statements:
    get:
      summary: Get Statements
      description: Get Statements
      operationId: GetStatements
      x-api-path-slug: statements-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statements
---