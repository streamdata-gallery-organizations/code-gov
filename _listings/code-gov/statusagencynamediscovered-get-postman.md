{
  "info": {
    "name": "Code.gov Get a list of repos by agency",
    "_postman_id": "86f3c92f-d540-4723-b1dd-c2f1a6c95424",
    "description": "Get a list of repos by agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "1c6585ca-b4a9-432e-ac67-8812b98efe0b",
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
              "id": "2bcc6b93-b2f4-424c-ac98-305867db9a67"
            }
          ]
        },
        {
          "id": "23b4f905-ad78-478c-8bfb-26cb3e5cfa6c",
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
              "id": "8dbc0a32-a97f-4eb7-b2ba-0fea6f9e8d13"
            }
          ]
        },
        {
          "id": "308ff8f3-f8b5-476f-9d26-3ffd87e020d5",
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
              "id": "5855ca39-c55f-4189-87cb-2bba9a73ab0f"
            }
          ]
        },
        {
          "id": "4a87920f-6581-4a85-beb0-70da24a82472",
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
              "id": "b4e8a212-692e-420a-a14b-cc9aa74be5cc"
            }
          ]
        },
        {
          "id": "b03161fa-e026-4f73-8bc6-41c5477435f7",
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
              "id": "4787cfa0-0cf0-4884-8a6b-af301c3c28e0"
            }
          ]
        },
        {
          "id": "38dffefe-57dc-454b-a34e-67da9af0b6eb",
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
              "id": "d41f7fa0-dde9-4699-8992-c0e66e0d44cb"
            }
          ]
        },
        {
          "id": "bf0fd4e8-9e6e-4319-908d-3d32a257b42f",
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
              "id": "eb50128b-9120-47a6-9814-f38bb3f7fc5a"
            }
          ]
        },
        {
          "id": "ca6df254-52f5-4866-a1d1-1bd74ee45c40",
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
              "id": "b5bca79c-3df2-4804-83fd-e95b07313a71"
            }
          ]
        },
        {
          "id": "915f5de5-c756-4ea4-80f1-4f931701d668",
          "name": "getStatusAgencynameDiscovered",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/discovered"
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
            "description": "Get a list of repos by agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d750e099-96e2-4d6c-a4e5-488070a389be"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "e1a2a85c-5772-42eb-a30a-5db801cd9b7a",
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
              "id": "723d70b5-8101-4f81-a799-52c0d59091a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "f5c54009-ee84-4da0-8e7c-7b51c8548f24",
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
              "id": "ee1b783c-8506-4b8e-a9cd-59e781b608f4"
            }
          ]
        }
      ]
    }
  ]
}