---
swagger: "2.0"
x-collection-name: Code.gov
x-complete: 0
info:
  title: Code.gov Get a list of agencies with their compliance status
  description: Get a list of agencies with their Federal Source Code Policy compliance
    status
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos:
    get:
      summary: Get a list of repos
      description: Get list of repositories indexed by Code.gov.
      operationId: getRepos
      x-api-path-slug: repos-get
      parameters:
      - in: query
        name: agency.acronym
        description: Filters search by the Agencys acronym
      - in: query
        name: agency.name
        description: Filters search by the Agencys name
      - in: query
        name: agency.website
        description: Filters search by the Agencys website URL
      - in: query
        name: contact.email
        description: Filters search by the repositorys contact email
      - in: query
        name: contact.name
        description: Filters search by the repositorys contact name
      - in: query
        name: date.created
        description: Filters search by the repositorys created date
      - in: query
        name: date.lastModified
        description: Filters search by the last date the repository was modified
      - in: query
        name: from
        description: Sets the offset from where to paginate
      - in: query
        name: laborHours
        description: Filters search by the amount of labor hours dedicated to the
          project
      - in: query
        name: languages
        description: Filters search by programming languages
      - in: query
        name: name
        description: Filters search by the repositorys name
      - in: query
        name: organization
        description: Filters search by the repositorys organization
      - in: query
        name: permissions.licenses.name
        description: Filters search by the repositorys license name
      - in: query
        name: permissions.usageType
        description: Filters search by the repositorys usage type
      - in: query
        name: q
        description: Text to search for
      - in: query
        name: size
        description: Sets the size of the results returned
      - in: query
        name: status
        description: Filters search by the repositorys status
      - in: query
        name: tags
        description: Filters search by the repositorys tags
      - in: query
        name: vcs
        description: Filters search by the version control system for the repository
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /repos/{repoId}:
    get:
      summary: Get information for specified repoId
      description: Gets the information of a specific repository index with the passed
        repoId.
      operationId: getReposRepo
      x-api-path-slug: reposrepoid-get
      parameters:
      - in: path
        name: repoId
        description: ID of repo to return
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /terms:
    get:
      summary: Get a list of terms
      description: Get a list of terms that were extracted from the repositories indexed.
      operationId: getTerms
      x-api-path-slug: terms-get
      parameters:
      - in: query
        name: from
        description: Sets the offset from where to paginate
      - in: query
        name: size
        description: Sets the size of the results returned
      - in: query
        name: term
        description: Filters the result set by the term value
      - in: query
        name: term_type
        description: Filters the result set by the term type
      responses:
        200:
          description: OK
      tags:
      - Code
      - Terms of Service
  /agencies:
    get:
      summary: Get a list of agencies
      description: Get a list of agencies.
      operationId: getAgencies
      x-api-path-slug: agencies-get
      parameters:
      - in: query
        name: from
        description: Specify an offset to return
      - in: query
        name: size
        description: Number of agencies to return
      responses:
        200:
          description: OK
      tags:
      - Agencies
  /languages:
    get:
      summary: Get a list of programming languages found in our code inventory.
      description: This returns a list of the programming languages that are used
        in the indexed code inventory. When a repo is index the programming language
        is extracted written to a file.
      operationId: getLanguages
      x-api-path-slug: languages-get
      parameters:
      - in: query
        name: from
        description: Specify an offset to return
      - in: query
        name: size
        description: Number of programming languages to return
      responses:
        200:
          description: OK
      tags:
      - Languages
  /repo.json:
    get:
      summary: Get the JSON schema for a repo
      description: Get the json schema for a repo.
      operationId: getRepo
      x-api-path-slug: repojson-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /status.json:
    get:
      summary: Get a list of agencies with their compliance status
      description: Get a list of agencies with their Federal Source Code Policy compliance
        status
      operationId: getStatus.json
      x-api-path-slug: statusjson-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---