{
  "info": {
    "name": "Open Bank Project Get Scheduled Payments",
    "_postman_id": "4e877cbb-1edd-4856-9596-e261913d4001",
    "description": "Get Scheduled Payments",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Banking",
      "item": [
        {
          "id": "b485db4d-f31a-492a-b401-2b638ec78a40",
          "name": "CreateAccountRequest",
          "request": {
            "url": "{{default}}/account-requests?No Name=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d83f689-bd80-4996-944d-ed025601711c"
            }
          ]
        },
        {
          "id": "a0753790-264c-4d80-94c1-426edc23cf3e",
          "name": "GetAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69df2cad-df49-4c53-9f42-223ced3606b7"
            }
          ]
        },
        {
          "id": "861f58f0-1857-4489-8059-b2644f062508",
          "name": "DeleteAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d667e046-295e-4f98-a5fa-1b5216bd8ab8"
            }
          ]
        },
        {
          "id": "9a1844bf-a4a6-4c61-8a0e-366d6944a02b",
          "name": "GetAccounts",
          "request": {
            "url": "{{default}}/accounts?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53782b39-8690-4622-87b3-2d78b013fbc3"
            }
          ]
        },
        {
          "id": "106a0b03-32bf-4cbc-9b32-200d280e1edb",
          "name": "GetAccount",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2bf8859-1444-41f2-9474-3818c9bb4858"
            }
          ]
        },
        {
          "id": "102cbc11-a515-46a4-9d3a-90ca0edcfcec",
          "name": "GetAccountTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20b24cfb-60be-4976-bd87-50d1ae0fb648"
            }
          ]
        },
        {
          "id": "52f84c76-5a60-4721-ae06-5adffe83fc41",
          "name": "GetAccountBeneficiaries",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/beneficiaries"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5524c6c3-e40c-4b0f-b7d7-9dcf1196d1b2"
            }
          ]
        },
        {
          "id": "4c59f42b-9520-4943-a2bc-e300b91f623e",
          "name": "GetAccountBalances",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/balances"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31826316-4631-4cf3-b1b9-f9c1e6bebd76"
            }
          ]
        },
        {
          "id": "e91721ec-b8d2-42aa-be3e-9395e23132fb",
          "name": "GetAccountDirectDebits",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/direct-debits"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ad4da05-abdc-469d-ad00-9f918b96f2b6"
            }
          ]
        },
        {
          "id": "cf179395-30e1-4729-8a09-53d838551e1a",
          "name": "GetAccountStandingOrders",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/standing-orders"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "222f67da-0903-4e3b-9caf-be4d393d824b"
            }
          ]
        },
        {
          "id": "ce9ac3a5-7c3e-4340-867a-23dab01ef20b",
          "name": "GetAccountProduct",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/product"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Product related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15f37e8e-475e-4a48-8afa-4b75bb8fbc8e"
            }
          ]
        },
        {
          "id": "517da0d5-30a5-4a86-b28c-3721188ef50d",
          "name": "GetAccountOffers",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/offers"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b25c6d8e-ce44-46d3-8b96-7db86e181fda"
            }
          ]
        },
        {
          "id": "06cc71bd-f467-4a83-9680-e5055ecf5665",
          "name": "GetAccountParty",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/party"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f187a971-bcb6-46a4-9943-b2f33c70599b"
            }
          ]
        },
        {
          "id": "1ac770e2-c414-49b0-8e96-84b9cce4685d",
          "name": "GetAccountScheduledPayments",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/scheduled-payments"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad6312a4-1ce7-4b82-9a15-af1c3d41938c"
            }
          ]
        },
        {
          "id": "6b763800-f50e-4546-8a4f-699d4243279c",
          "name": "GetAccountStatements",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f748075d-7fa5-44b7-9341-7685cc1b6efe"
            }
          ]
        },
        {
          "id": "8199717a-0521-48bf-b3c5-dbd9b55c752c",
          "name": "GetAccountStatement",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54a386fc-59d2-431f-b5cc-a6dacd53afa4"
            }
          ]
        },
        {
          "id": "c786e07e-a6a8-4623-8dc0-40ae8efd6113",
          "name": "GetAccountStatementFile",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/file"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement File related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23cfe122-5e24-482f-8788-c516a639bb16"
            }
          ]
        },
        {
          "id": "62bb5f4a-61c2-40c4-a3ec-b896bedd730e",
          "name": "GetAccountStatementTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement Transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63c77005-c5b4-4272-92fa-63813f6d5dea"
            }
          ]
        },
        {
          "id": "fd1b9e62-9822-4569-9a26-cdd4b7666a82",
          "name": "GetStandingOrders",
          "request": {
            "url": "{{default}}/standing-orders?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5c644e6-3e07-484b-97fb-5374a9451b0f"
            }
          ]
        },
        {
          "id": "a88407df-3c73-40d3-afb1-ec73f15b7114",
          "name": "GetDirectDebits",
          "request": {
            "url": "{{default}}/direct-debits?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d3f3fe6-49bb-4d7a-bfac-9f9c10dc4a6a"
            }
          ]
        },
        {
          "id": "259de7cc-7c78-4f3a-83f9-dfeaba5ae9a5",
          "name": "GetBeneficiaries",
          "request": {
            "url": "{{default}}/beneficiaries?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c809293-8678-42f4-a7f2-f31943636f62"
            }
          ]
        },
        {
          "id": "2e646740-04f2-46d1-9628-84bc2cced716",
          "name": "GetTransactions",
          "request": {
            "url": "{{default}}/transactions?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e71d5f8f-6082-4401-9487-6977ce2b592c"
            }
          ]
        },
        {
          "id": "30fbe8ed-80e2-43fd-af48-59f183359656",
          "name": "GetBalances",
          "request": {
            "url": "{{default}}/balances?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0d2e074-9af4-460c-9d43-c5fe7bf8d017"
            }
          ]
        },
        {
          "id": "dd4d484c-0685-4616-93f3-0df93d813034",
          "name": "GetProducts",
          "request": {
            "url": "{{default}}/products?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Products"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55f429bc-75ab-409c-9399-c5c6f560e21b"
            }
          ]
        },
        {
          "id": "c99dedec-649e-429a-aae9-f3ee5b0f777a",
          "name": "GetOffers",
          "request": {
            "url": "{{default}}/offers?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6058fa9b-7763-4a48-a6ae-3e18b43f9efc"
            }
          ]
        },
        {
          "id": "df2644b3-87f6-4fb5-b067-7a1ebabc8d1a",
          "name": "GetParty",
          "request": {
            "url": "{{default}}/party?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69a9f79c-5ace-4828-8d88-feabbde60226"
            }
          ]
        },
        {
          "id": "70b3956c-fc53-4161-803a-a8a62d87c8fe",
          "name": "GetScheduledPayments",
          "request": {
            "url": "{{default}}/scheduled-payments?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b17f5582-8469-46d9-b43b-e3fec2f77a7f"
            }
          ]
        },
        {
          "id": "8072b4eb-8d77-47c4-9ba1-d57f20e6746c",
          "name": "GetStatements",
          "request": {
            "url": "{{default}}/statements?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bf22861-d88a-4746-a946-b0efc113d729"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/open-banking/v2.0"
    }
  ]
}