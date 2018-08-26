{
  "info": {
    "name": "Open Bank Project Get Offers",
    "_postman_id": "6069bf12-2607-453b-b584-42a97e064a57",
    "description": "Get Offers",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Banking",
      "item": [
        {
          "id": "f7036b5e-4c0c-414f-a97a-3f0b4a2d3b39",
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
              "id": "d5b92b19-4db8-4e05-a6a4-9ceedc1133f8"
            }
          ]
        },
        {
          "id": "cac2eddb-f58f-4189-9be0-f9fc991f387d",
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
              "id": "83bd14a2-c6ac-40e4-bc7e-d03118784830"
            }
          ]
        },
        {
          "id": "c348bc3a-c701-4169-bc07-aa25ed2f954d",
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
              "id": "9b37ebf9-9d29-4f8b-b500-8742ce342af7"
            }
          ]
        },
        {
          "id": "46402ffd-71d6-4673-88cb-d9c69e09e1d2",
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
              "id": "00e1f5a4-1972-4e0f-a236-ff713642aa96"
            }
          ]
        },
        {
          "id": "f9d5f2a2-a55b-4ab1-937e-abf0df18aa2a",
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
              "id": "a7167d23-08bb-4b2b-8dd8-190ba227d413"
            }
          ]
        },
        {
          "id": "dec4b399-2e87-444f-93b4-6677e701269c",
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
              "id": "6973b516-13f0-499d-9c34-e2880228e4ce"
            }
          ]
        },
        {
          "id": "bf62ce0c-6270-487f-928d-2d0cafbb1b1d",
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
              "id": "19dca6f1-b858-4bdd-b64d-04ed40b8afe6"
            }
          ]
        },
        {
          "id": "0d53baf2-2120-4e67-a4db-264df9a114ea",
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
              "id": "4243b13d-758c-48f6-bad0-7faaf125c7bf"
            }
          ]
        },
        {
          "id": "86a86bc6-302c-4c4b-8e15-f92a7479ca16",
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
              "id": "ca2d8e5d-2cae-487b-ace8-d8e09367a75c"
            }
          ]
        },
        {
          "id": "aea51a1c-86ac-419a-8994-fb008793428a",
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
              "id": "f6a877fe-fc9f-454d-9058-bfd3f80a9284"
            }
          ]
        },
        {
          "id": "032bb92c-e367-4b2a-ad60-8bd20aa5e1bf",
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
              "id": "46dab3ae-64ce-4b85-95bf-51b6473eaada"
            }
          ]
        },
        {
          "id": "ae4746f5-d760-4a57-816d-c92b2e5f4cec",
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
              "id": "08ab5d28-7349-47eb-a006-e810b6eca4a2"
            }
          ]
        },
        {
          "id": "42a41fc8-6dbc-45c3-8219-dae47e950496",
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
              "id": "24d319b8-7ec3-4084-bcb4-60f86b0911d7"
            }
          ]
        },
        {
          "id": "0faba7bc-d0e8-46b3-b5d8-9e9cc502d7da",
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
              "id": "c4a2617d-f479-4c36-8080-20401a3c6531"
            }
          ]
        },
        {
          "id": "17dfc084-09c4-4e0e-b9e5-09bcbd31ef37",
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
              "id": "ddc24ca0-738f-47cb-b6be-6ca10921e9a1"
            }
          ]
        },
        {
          "id": "133c3d4b-19c9-42fa-ba57-ae0a63562470",
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
              "id": "0305fe29-094d-4d41-82e5-a9d6f8198d26"
            }
          ]
        },
        {
          "id": "e5cf9a95-bbd8-4fc8-80f2-9f0f8eeab172",
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
              "id": "376e9e36-0cc7-416f-9858-86d1b95738f3"
            }
          ]
        },
        {
          "id": "16d29b14-0558-4c44-bd8f-8dee7181238a",
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
              "id": "e6c494d2-fc37-4445-8d95-36380800134f"
            }
          ]
        },
        {
          "id": "d0aff86d-780f-4f81-a980-cd6c13c2ca41",
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
              "id": "826539e7-6246-4e8f-9708-41c740002c86"
            }
          ]
        },
        {
          "id": "bbfd79bb-7785-4d96-b628-7cc26ab105a2",
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
              "id": "1ca9b5ab-ac11-4b74-933a-1761b84d0d10"
            }
          ]
        },
        {
          "id": "27192fad-b238-4e34-bef8-3c6fbe1e1dd7",
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
              "id": "3e8d531a-a7fa-4087-ac2e-ba6fd32104f8"
            }
          ]
        },
        {
          "id": "54adbbba-7618-46d4-83d0-481c7daa1fab",
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
              "id": "e8f69959-c6c3-4aab-8fe3-cf253f7baabf"
            }
          ]
        },
        {
          "id": "b8bb31a9-51b0-4cfd-8d3f-2f48f462f06f",
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
              "id": "af5c7a01-3e3f-4e39-ad5e-ca23faa179a8"
            }
          ]
        },
        {
          "id": "4b0d577e-ba12-41ed-8db5-f96ea9da7172",
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
              "id": "ed566004-6302-488a-9775-7c10ed48acfe"
            }
          ]
        },
        {
          "id": "1c62c2a2-c762-4a33-b71e-ad54d911f05d",
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
              "id": "7a1074e7-6ccf-4ee9-a1d7-51feaff586e9"
            }
          ]
        },
        {
          "id": "f770980f-9690-414a-b784-4c25191435a0",
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
              "id": "08751c27-1408-4426-9ded-f799ee09379c"
            }
          ]
        },
        {
          "id": "3291537e-4a0f-4967-8873-c3f2a3ba35fa",
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
              "id": "e29bab63-b65e-4d97-bd67-52f8bd9391da"
            }
          ]
        },
        {
          "id": "05d2cc48-fde6-43f4-ab0f-ee51d1596e09",
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
              "id": "7ccdc122-68c4-4c13-97e1-6e181b28f0a7"
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