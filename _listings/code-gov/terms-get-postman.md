{
  "info": {
    "name": "Code.gov Get a list of terms",
    "_postman_id": "ce3e3c2e-97e9-44fb-87bc-444b81d1127f",
    "description": "Get a list of terms that were extracted from the repositories indexed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "0782cd9a-c41c-4b13-97c2-614bcb1d351b",
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
              "id": "7e6735d9-215a-4f52-9952-7f93c6bd34b0"
            }
          ]
        },
        {
          "id": "b4d4d75e-1c99-4912-980e-28f29fbaaa3d",
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
              "id": "870cd36e-db7e-45b6-a4b9-e55c6c06fbb2"
            }
          ]
        },
        {
          "id": "3bc7cc4d-a008-4f72-9845-632e4aa5fd58",
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
              "id": "49b70e0b-6080-47e8-9032-bb8fe1f41e4e"
            }
          ]
        }
      ]
    }
  ]
}