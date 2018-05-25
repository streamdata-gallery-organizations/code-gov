{
  "info": {
    "name": "Code.gov Get an HTML page rendering the agencies status from status.json",
    "_postman_id": "378cda86-f681-48e7-b259-e1c3c6570fa6",
    "description": "Get an html page rendering the agencies status from status.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "d36a3e8b-40f6-4faa-8484-73efa1362c66",
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
              "id": "583a02d6-618a-4c28-b6e1-7ab33165b80d"
            }
          ]
        },
        {
          "id": "03929d30-9b02-4c16-9aa1-1319bc8e7145",
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
              "id": "e8d0c06b-5ab7-47a4-bdca-2bf00be8fd41"
            }
          ]
        },
        {
          "id": "90434302-9f1a-4728-bcd5-45c63fe4c5ae",
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
              "id": "6b388b05-3c58-4a2f-b2f2-1c3bd00c9f0d"
            }
          ]
        },
        {
          "id": "544c6c7d-024e-4780-a0db-2a383d90769a",
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
              "id": "4346fd34-37d3-4190-8daa-8162cf7bc2b6"
            }
          ]
        },
        {
          "id": "d841c145-5f5a-4293-b7a5-cef7cb8fcd28",
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
              "id": "19dd5e96-38ef-4ff7-9a6d-d38a9ce06ef5"
            }
          ]
        },
        {
          "id": "ad2b4b67-2708-41d9-b49b-dbc1633dd61c",
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
              "id": "ee41183d-5e3b-405d-964f-2139f46f3c4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "b7ecbbe7-7419-46ed-b051-f3cbf3e0c493",
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
              "id": "be9ff17f-fb97-47f1-a283-b41c397a9bc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "8738037e-16fc-4b0c-8dec-91d5b9ced894",
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
              "id": "5ee5dcf5-9568-4464-a94a-3d35ceadbf9a"
            }
          ]
        }
      ]
    }
  ]
}