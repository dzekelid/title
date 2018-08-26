---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Job Title Autocomplete
  description: Retrieves the names, descriptions, and UUIDs of all job titles matching
    a given search criteria.
  contact:
    name: Work Data Initiative
    url: http://www.dataatwork.org
  version: "1.0"
host: api.dataatwork.org
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{id}:
    get:
      summary: Job Title and Description
      description: Retrieves the name, description, and UUID of a job by specifying
        its O*NET SOC Code or UUID.
      operationId: retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-onet-soc-code-or-uuid
      x-api-path-slug: jobsid-get
      parameters:
      - in: path
        name: id
        description: The O*NET SOC Code or UUID of the job title to retrieve
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Description
  /jobs/autocomplete:
    get:
      summary: Job Title Autocomplete
      description: Retrieves the names, descriptions, and UUIDs of all job titles
        matching a given search criteria.
      operationId: retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria
      x-api-path-slug: jobsautocomplete-get
      parameters:
      - in: query
        name: begins_with
        description: Find job titles beginning with the given text fragment
      - in: query
        name: contains
        description: Find job titles containing the given text fragment
      - in: query
        name: ends_with
        description: Find job titles ending with the given text fragment
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Autocomplete
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