---
name: Code.gov
x-slug: codegov
description: Code.gov leverages the power of code sharing and collaboration to help
  the US Government cut down on duplicative software development and save millions
  of taxpayer dollars for the American people.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
x-kinRank: "7"
x-alexaRank: ""
tags: Code.gov
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/apis.md
specificationVersion: "0.14"
apis:
- name: Code.gov Get a list of repos
  x-api-slug: codegov
  description: Get list of repositories indexed by Code.gov.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////repos
  tags: Code,Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/repos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/repos-get-openapi.md
- name: Code.gov Get information for specified repoId
  x-api-slug: codegov
  description: Gets the information of a specific repository index with the passed
    repoId.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////repos/{repoId}
  tags: Code,Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/reposrepoid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/reposrepoid-get-openapi.md
- name: Code.gov Get a list of terms
  x-api-slug: codegov
  description: Get a list of terms that were extracted from the repositories indexed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////terms
  tags: Code,Terms of Service
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/terms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/terms-get-openapi.md
- name: Code.gov Get a list of agencies
  x-api-slug: codegov
  description: Get a list of agencies.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////agencies
  tags: Agencies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/agencies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/agencies-get-openapi.md
- name: Code.gov Get a list of programming languages found in our code inventory.
  x-api-slug: codegov
  description: This returns a list of the programming languages that are used in the
    indexed code inventory. When a repo is index the programming language is extracted
    written to a file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////languages
  tags: Languages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/languages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/languages-get-openapi.md
- name: Code.gov Get the JSON schema for a repo
  x-api-slug: codegov
  description: Get the json schema for a repo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////repo.json
  tags: Code,Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/repojson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/repojson-get-openapi.md
- name: Code.gov Get a list of agencies with their compliance status
  x-api-slug: codegov
  description: Get a list of agencies with their Federal Source Code Policy compliance
    status
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////status.json
  tags: Code,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusjson-get-openapi.md
- name: Code.gov Get an HTML page rendering the agencies status from status.json
  x-api-slug: codegov
  description: Get an html page rendering the agencies status from status.json.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////status
  tags: Code,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/status-get-openapi.md
- name: Code.gov Get a list of issues for a particular agency
  x-api-slug: codegov
  description: Get a list of issues for a particular agency. These issues are grouped
    by software repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////status/{agencyName}/issues
  tags: Code,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynameissues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynameissues-get-openapi.md
- name: Code.gov Get a list of repos by agency
  x-api-slug: codegov
  description: Lists out all repositories that have been indexed for a given agency.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////status/{agencyName}/fetched
  tags: Code,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynamefetched-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynamefetched-get-openapi.md
- name: Code.gov Get a list of repos by agency
  x-api-slug: codegov
  description: Get a list of repos by agency.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////status/{agencyName}/discovered
  tags: Code,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynamediscovered-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/statusagencynamediscovered-get-openapi.md
- name: Code.gov Get the version of this API
  x-api-slug: codegov
  description: Get the version of this api.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov////version
  tags: Code,Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/version-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/version-get-openapi.md
- name: Code.gov
  x-api-slug: codegov
  description: Code.gov leverages the power of code sharing and collaboration to help
    the US Government cut down on duplicative software development and save millions
    of taxpayer dollars for the American people.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/code-gov-logo.jpg
  humanURL: https://code.gov/
  baseURL: https://api.code.gov//
  tags: Code.gov
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/code.gov/master/_listings/codegov/openapi.md
x-common:
- type: x-applications
  url: https://code.gov/#/explore-code
- type: x-developer
  url: https://api.code.gov/docs/
- type: x-documentation
  url: https://api.code.gov/docs/#
- type: x-road-map
  url: https://code.gov/#/roadmap
- type: x-twitter
  url: https://twitter.com/codedotgov
- type: x-website
  url: https://code.gov/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---