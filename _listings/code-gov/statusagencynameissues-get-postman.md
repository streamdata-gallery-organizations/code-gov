{
  "info": {
    "name": "Code.gov Get a list of issues for a particular agency",
    "_postman_id": "88e7c218-c89f-4625-a9a9-589b038a8bc5",
    "description": "Get a list of issues for a particular agency. These issues are grouped by software repository.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "39bb3207-07c8-454c-b57e-009dddeb9550",
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
              "id": "54a12a4d-fba5-46b5-b7bf-fe652c88111c"
            }
          ]
        },
        {
          "id": "85b96bb8-8471-4e31-8c81-1a45ef58e9c8",
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
              "id": "777ebae8-56f5-4bed-bcde-e49aebf5c77e"
            }
          ]
        },
        {
          "id": "0a9e07fc-f921-4401-8d42-448062bbe470",
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
              "id": "8369ff52-3330-43ae-a7a0-4b0137ff3248"
            }
          ]
        },
        {
          "id": "c86351bd-0008-4a27-b8a3-14a49c5ababf",
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
              "id": "19937ec9-c5bf-4969-ab90-83191eb98433"
            }
          ]
        },
        {
          "id": "2fe9bbf5-3fe0-4439-8c03-4d658752f6c1",
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
              "id": "60c8b394-84ba-49f5-9b47-29abb0359edc"
            }
          ]
        },
        {
          "id": "509fc33d-08ff-43e2-b884-c0c029a2a671",
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
              "id": "b24ada08-a672-4a8f-96d5-9869392ba4ad"
            }
          ]
        },
        {
          "id": "645a306e-4f44-40d9-913a-a02ae87f7b64",
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
              "id": "86fb1048-749d-4a14-821e-ccc454b843c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "42351c2a-382b-4a98-af05-5933c4511a5d",
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
              "id": "503af61b-1faa-4dad-8465-e756c3784233"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "f02e2fb8-f515-4e3f-ac37-07049f77c2ea",
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
              "id": "ab11fe5f-ca51-4eaf-a97b-70950ddac8b1"
            }
          ]
        }
      ]
    }
  ]
}