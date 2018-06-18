{
  "info": {
    "name": "Standard Chartered Bank Code Inquiry",
    "_postman_id": "62da9556-6d8d-4b56-b7d3-77edb95e5741",
    "description": "The “GetBankCode” API returns list of Bank Codes for the specified combination of “Country”, “City” and “Bank” combination. The data will contain the “Bank Code(s)” as well as the address for the Bank & Branch.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "62de1ef2-e992-4508-9e97-407ab3bdb6f8",
          "name": "postCibServiceS2bApiV1BanksScbReferenceDefaultBranches",
          "request": {
            "url": "http://developer.sc.com/cib/service/s2b/api/v1/banks/scb/reference/default/branches",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The “GetBankCode” API returns list of Bank Codes for the specified combination of “Country”, “City” and “Bank” combination. The data will contain the “Bank Code(s)” as well as the address for the Bank & Branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e014660-1c92-4efd-964e-ead681da68d0"
            }
          ]
        }
      ]
    }
  ]
}