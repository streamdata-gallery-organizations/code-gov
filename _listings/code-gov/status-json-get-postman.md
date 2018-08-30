{
  "info": {
    "name": "Code.gov Get a list of agencies with their compliance status",
    "_postman_id": "25b736b0-5b27-4d1a-a9ca-7655d9642777",
    "description": "Get a list of agencies with their Federal Source Code Policy compliance status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "99f2722a-e308-4052-85ea-63445e73ba74",
          "name": "getRepos",
          "request": {
            "url": "http://api.code.gov/repos?agency.acronym=%7B%7D&agency.name=%7B%7D&agency.website=%7B%7D&contact.email=%7B%7D&contact.name=%7B%7D&date.created=%7B%7D&date.lastModified=%7B%7D&from=%7B%7D&laborHours=%7B%7D&languages=%7B%7D&name=%7B%7D&organization=%7B%7D&permissions.licenses.name=%7B%7D&permissions.usageType=%7B%7D&q=%7B%7D&size=%7B%7D&status=%7B%7D&tags=%7B%7D&vcs=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get list of repositories indexed by Code.gov."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c598270f-6af4-483a-bfab-c5ffc6652f0e"
            }
          ]
        },
        {
          "id": "cbb373a3-962a-4faa-9534-6a5e71edde49",
          "name": "getReposRepo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "repos/:repoId"
              ],
              "variable": [
                {
                  "id": "repoId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the information of a specific repository index with the passed repoId."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cecbae4-61b7-4bc6-9613-53e30163f5c4"
            }
          ]
        },
        {
          "id": "0c57b40a-863a-4360-8c37-f273305fd14f",
          "name": "getTerms",
          "request": {
            "url": "http://api.code.gov/terms?from=%7B%7D&size=%7B%7D&term=%7B%7D&term_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of terms that were extracted from the repositories indexed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fd378ab-1dd3-46ed-b8df-bab7650ba17f"
            }
          ]
        },
        {
          "id": "e7b8136d-3bda-491a-a377-67d3d940e39c",
          "name": "getRepo",
          "request": {
            "url": "http://api.code.gov/repo.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the json schema for a repo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40617976-a362-4b27-98bc-372c66d41199"
            }
          ]
        },
        {
          "id": "4bfb8c33-11ae-4bcb-8fd7-3606dcd9913d",
          "name": "getStatus.json",
          "request": {
            "url": "http://api.code.gov/status.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of agencies with their Federal Source Code Policy compliance status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1041331-a9a1-4a08-8ab7-b71579b89123"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "039c49fa-9126-4235-9dba-c3397a5b3d1f",
          "name": "getAgencies",
          "request": {
            "url": "http://api.code.gov/agencies?from=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of agencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cd0e944-a4f1-4f18-85f7-0d855a861683"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "00438e08-0c7b-4f44-922d-ba4ba99b1087",
          "name": "getLanguages",
          "request": {
            "url": "http://api.code.gov/languages?from=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This returns a list of the programming languages that are used in the indexed code inventory. When a repo is index the programming language is extracted written to a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d167cc9e-ae99-41c3-b61b-48f5d3c29621"
            }
          ]
        }
      ]
    }
  ]
}