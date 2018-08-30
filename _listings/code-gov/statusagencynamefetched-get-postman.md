{
  "info": {
    "name": "Code.gov Get a list of repos by agency",
    "_postman_id": "d9998c65-a486-43bc-8b04-3ae6ee16701d",
    "description": "Lists out all repositories that have been indexed for a given agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "bc8f93d9-ba2c-4e3c-a7ae-798ef4e25bf2",
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
              "id": "18e084bc-28ad-4616-bb46-20cd70551eb6"
            }
          ]
        },
        {
          "id": "ee288a21-d971-4df0-827f-20270252cac8",
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
              "id": "810f3eba-6d50-48ca-88b9-6738b54fb625"
            }
          ]
        },
        {
          "id": "748e8364-15a7-44bd-99bc-0e19417e7cf9",
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
              "id": "f833f14c-d19c-42b2-afa2-19e1bad438d1"
            }
          ]
        },
        {
          "id": "1c390df4-a5ac-4945-9a39-477d9e95d513",
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
              "id": "60925d71-306e-4a86-8475-ab31970fb3e6"
            }
          ]
        },
        {
          "id": "08557994-5724-4f9e-9c86-8de9591ab090",
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
              "id": "a6296dd2-d69d-45c7-827e-99f48c2eb89d"
            }
          ]
        },
        {
          "id": "f9834cf6-af6e-4081-85e0-7e047095e119",
          "name": "getStatus",
          "request": {
            "url": "http://api.code.gov/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an html page rendering the agencies status from status.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f958f75-9025-4218-a7a3-6263d4b3022a"
            }
          ]
        },
        {
          "id": "3ba38ec1-107e-469a-b0b2-fedfd5a059a3",
          "name": "getStatusAgencynameIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/issues"
              ],
              "variable": [
                {
                  "id": "agencyName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of issues for a particular agency. These issues are grouped by software repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2804cad0-8762-4892-9942-b641afce5e55"
            }
          ]
        },
        {
          "id": "1b3ef3e7-4e39-4297-8592-d5e95fb1e463",
          "name": "getStatusAgencynameFetched",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/fetched"
              ],
              "variable": [
                {
                  "id": "agencyName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists out all repositories that have been indexed for a given agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56e43792-7850-45f9-866c-b93795305f90"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "b1b00a65-b5ae-46e3-ba0f-e01403947cb9",
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
              "id": "66c94292-d386-4531-aa00-799b16444f92"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "36fdab5f-c9ed-4015-9151-155f2593e659",
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
              "id": "6fd2d68b-9036-4626-a3bc-1deb075e1f11"
            }
          ]
        }
      ]
    }
  ]
}