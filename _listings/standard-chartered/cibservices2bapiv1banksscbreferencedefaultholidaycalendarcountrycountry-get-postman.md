{
  "info": {
    "name": "Standard Chartered Holiday Calendar Inquiry (Country)",
    "_postman_id": "47cebfa6-c293-4ebc-8a52-211c6356888c",
    "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Country</li><li>Date Range</li></lu>",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "08743890-c2de-45c6-9d45-bb75550cd7e9",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/account"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetAccountBalance??? API upon successful user authentication and entitlement checks will return the various types of ???Account Balances??? applicable for the specified Account Number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4d9cbae-173f-428a-a3ad-75d20cfd7d8b"
            }
          ]
        },
        {
          "id": "de3fb956-c1b0-4e5c-b8eb-48a6fdb182a4",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewTransactionRequestTypes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/transaction-request-types"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetTransactionTypes??? API upon successful user authentication and entitlement checks will return the supported transaction types for the specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8622d25-d76a-44ab-886b-a96bcf3b0e8b"
            }
          ]
        },
        {
          "id": "92f6dbd8-421d-4055-9438-e7a1522576f9",
          "name": "getCibServiceS2bApiV1BanksScbAccountsViewAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:viewId/accounts"
              ],
              "variable": [
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List available bank accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "443779d8-9654-46cf-9919-d5e0b1f15020"
            }
          ]
        },
        {
          "id": "e83226eb-fa05-4e42-bb15-e7356d964372",
          "name": "postCibServiceS2bApiV1BanksScbReferenceDefaultBranches",
          "request": {
            "url": "http://developer.sc.com/cib/service/s2b/api/v1/banks/scb/reference/default/branches",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetBankCode??? API returns list of Bank Codes for the specified combination of ???Country???, ???City??? and ???Bank??? combination. The data will contain the ???Bank Code(s)??? as well as the address for the Bank & Branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44c842b5-f06a-4943-a3ee-23da1d0fee13"
            }
          ]
        },
        {
          "id": "7ed9b92f-49b3-40cd-a2bf-2ee086664604",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCountryCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/country/:country"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Country</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5554e96e-a8c5-46cc-a828-4c557b9ee6cc"
            }
          ]
        }
      ]
    }
  ]
}