---
name: DataAtWork
x-slug: dataatwork
description: ""
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2016-10-12 at 11.19.25 PM.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Title
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/apis.md
specificationVersion: "0.14"
apis:
- name: Open Skills API - Job Title and Description
  x-api-slug: jobsid-get
  description: Retrieves the name, description, and UUID of a job by specifying its
    O*NET SOC Code or UUID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1
  tags: Federal Government, Careers, Skills, API Service Provider, Profiles, General
    Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsid-get-openapi.md
- name: Open Skills API - Job Title Autocomplete
  x-api-slug: jobsautocomplete-get
  description: Retrieves the names, descriptions, and UUIDs of all job titles matching
    a given search criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1
  tags: Federal Government, Careers, Skills, API Service Provider, Profiles, General
    Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsautocomplete-get-openapi.md
- name: Open Skills API - Job Title Normalization
  x-api-slug: jobsnormalize-get
  description: Retrieves the canonical job title for a synonymous job title
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1
  tags: Federal Government, Careers, Skills, API Service Provider, Profiles, General
    Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsnormalize-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/title/master/_listings/dataatwork/jobsnormalize-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://data2crm.api.gallery.streamdata.io
- type: x-api-stack
  url: http://dataatwork.stack.network
- type: x-developer
  url: http://api.dataatwork.org/v1/spec/
- type: x-website
  url: http://www.dataatwork.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---