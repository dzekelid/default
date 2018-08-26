{
  "info": {
    "name": "Standard Chartered Holiday Calendar Inquiry (Currency)",
    "_postman_id": "c6a1a5f4-d153-4e36-8b36-f13a8a8a92e2",
    "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Currency</li><li>Date Range</li></lu>",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "04e3884f-6e72-4c61-873c-697389811d65",
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
              "id": "20be0a2d-dd92-4ab2-8e90-98f8fc802b06"
            }
          ]
        },
        {
          "id": "20f901ab-f1e3-4880-b0b6-f30ea29fa594",
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
              "id": "98b76227-f89c-461d-b85d-c5eee9898474"
            }
          ]
        },
        {
          "id": "ef79c33e-4f20-4c00-ae75-f3ba22807927",
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
              "id": "c8c5e557-7d70-4566-8c24-91a1f1707ba4"
            }
          ]
        },
        {
          "id": "df0d4129-b4f5-4155-9aad-39bac78e96df",
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
              "id": "90a86b7a-80d8-4e3e-9d25-fca6fe7eeabd"
            }
          ]
        },
        {
          "id": "eb044712-58a5-490a-92c7-0f4f73386db3",
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
              "id": "3068f075-f3ce-4910-8089-e1fb565180bd"
            }
          ]
        },
        {
          "id": "f0e1a984-6f5b-412c-989e-fd96f737a99f",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCurrencyCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/currency/:currency"
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
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Currency</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99d4a5c0-b82c-46d2-bc97-2105e30b1eb6"
            }
          ]
        }
      ]
    }
  ]
}