{
  "info": {
    "name": "Open Bank Project Get Balances",
    "_postman_id": "cf68b9db-391c-4651-bebb-c9ec0db405f3",
    "description": "Get Balances",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Banking",
      "item": [
        {
          "id": "4a45a32f-a30e-4283-a098-ae1f62ddcdf3",
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
              "id": "c025bb6f-4cd8-4f38-8d89-3a5671d97688"
            }
          ]
        },
        {
          "id": "55e5632d-3db4-494a-a5f0-5528339b6b26",
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
              "id": "1ea67635-4fc6-4d8c-9279-7dce017a15ee"
            }
          ]
        },
        {
          "id": "2cf6c018-3001-4b06-9044-f605187d234b",
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
              "id": "998b0157-38e3-409d-a408-ae3cad20e3ed"
            }
          ]
        },
        {
          "id": "85ce3196-bd6e-4ff4-b4d8-6cec0c497063",
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
              "id": "0073994d-bcef-4b35-a905-45d049b79cea"
            }
          ]
        },
        {
          "id": "3139b268-6daf-4f63-9a02-04e641d98e23",
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
              "id": "b6cdd93a-789a-4bf5-a9ae-973b9618eb81"
            }
          ]
        },
        {
          "id": "a004d1c4-0429-4af7-ae12-c7b112292b09",
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
              "id": "c0532733-41ad-450c-ac48-1f2cfae6404d"
            }
          ]
        },
        {
          "id": "2e166136-8ec6-45d7-8c8e-fa42e4a9156d",
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
              "id": "77584b67-f709-4156-91dd-01c0cb43875c"
            }
          ]
        },
        {
          "id": "5479337c-526f-40b5-8f3d-5ea67eca05aa",
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
              "id": "d4c0471c-1497-4ed1-86b8-f46b1acf4b33"
            }
          ]
        },
        {
          "id": "7fcbbfcf-6ae6-48bb-8c92-ff054c215e33",
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
              "id": "334ff4d7-a722-4de0-9e58-3471d2cc3642"
            }
          ]
        },
        {
          "id": "3be745bb-5e6d-4f7c-8814-52362bf5304c",
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
              "id": "184b9b23-b0d2-4b81-878d-e52f1d02527c"
            }
          ]
        },
        {
          "id": "402d8594-b4cd-45db-9bb9-97e6f4f859d4",
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
              "id": "efba8ec0-70e8-490a-b5c7-af7224d7e205"
            }
          ]
        },
        {
          "id": "218b7d03-bd6d-458d-be38-25f45ecb32ea",
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
              "id": "536464d9-a97d-4d46-be95-c25d0bd07234"
            }
          ]
        },
        {
          "id": "c0931d2a-446e-40c5-8b09-6bd05bf14d63",
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
              "id": "cab3793b-3278-4a51-87b8-695c4fe29db2"
            }
          ]
        },
        {
          "id": "acf440f9-4249-4415-9124-bc34700d5ed1",
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
              "id": "5894c7ab-78be-43d2-804c-f30c00bc21d2"
            }
          ]
        },
        {
          "id": "6862cd62-f271-4814-aad8-2615ea52c6e9",
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
              "id": "315c7849-412f-49b0-be8b-bcb4715762f3"
            }
          ]
        },
        {
          "id": "91e965f0-3cfc-45e0-873f-4d3d9046f511",
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
              "id": "98872628-7bea-4535-a142-e70c52269453"
            }
          ]
        },
        {
          "id": "75259aca-184e-4963-8288-1f82c3dcaefb",
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
              "id": "7eba559c-5275-450a-a9de-1a78943d789b"
            }
          ]
        },
        {
          "id": "d1d23325-854d-4f2f-aedb-b4b40dc4357e",
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
              "id": "0565f862-16a0-458b-bc65-80fc0ec7c2cf"
            }
          ]
        },
        {
          "id": "760a2aba-7611-45f7-a500-d897b646840e",
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
              "id": "3fbe0728-d704-490d-8358-20ea466d237e"
            }
          ]
        },
        {
          "id": "2158e618-85c8-470a-a633-9de89dd436b7",
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
              "id": "ddd1627b-ed53-44aa-ab19-c328d8c53aec"
            }
          ]
        },
        {
          "id": "4071c7b1-8fb8-438f-9715-5fdb9a093191",
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
              "id": "234cb4a8-5ca4-49a4-9b74-f03d0293f336"
            }
          ]
        },
        {
          "id": "50aa50f3-f720-436f-b108-962103764e37",
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
              "id": "fdc2e783-eb64-4374-a085-e543de169173"
            }
          ]
        },
        {
          "id": "abaa89ee-82a3-4abb-beab-56d7d7ffe5a3",
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
              "id": "3c253cd7-7ebb-4091-abd7-c2dba2b42971"
            }
          ]
        },
        {
          "id": "a8b15845-8ded-4fa9-ab46-ba3845936f51",
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
              "id": "97619ec4-cd6a-4efa-80b5-238f3751d459"
            }
          ]
        },
        {
          "id": "dd24c363-630a-4338-a68d-11d76fef980c",
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
              "id": "b028aeb4-06cc-47fe-8436-5a9fd60b933b"
            }
          ]
        },
        {
          "id": "37198149-c8cb-4f67-bddc-3639b41e6c16",
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
              "id": "e5cdc8cf-df22-4823-a26f-2ce3a3e9e5cf"
            }
          ]
        },
        {
          "id": "691a26c7-7532-4c4f-8c11-9f7d0ab3507c",
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
              "id": "45cc152a-424c-49f2-9b44-a6908296523d"
            }
          ]
        },
        {
          "id": "78ea1371-adad-4990-85fa-b069ef414406",
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
              "id": "7f7fbeb9-2bb3-46dc-9986-9ca8a18da17f"
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