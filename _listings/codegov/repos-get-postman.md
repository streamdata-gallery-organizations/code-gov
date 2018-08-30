{
  "info": {
    "name": "Code.gov Get a list of repos",
    "_postman_id": "ce8e5bdc-2215-41d1-94b1-9c393650177f",
    "description": "Get list of repositories indexed by Code.gov.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "8d5349c8-f3b9-4d4f-a3cf-38f357118cca",
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
              "id": "694c40b9-10bd-4185-bcbb-26d7eaa662c8"
            }
          ]
        }
      ]
    }
  ]
}