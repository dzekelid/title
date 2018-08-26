---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 1
info:
  title: Open Skills API
  description: a-complete-and-standard-data-store-for-canonical-and-emerging-skills-knowledge-abilities-tools-technolgies-and-how-they-relate-to-jobs-
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
  /jobs/normalize:
    get:
      summary: Job Title Normalization
      description: Retrieves the canonical job title for a synonymous job title
      operationId: retrieves-the-canonical-job-title-for-a-synonymous-job-title
      x-api-path-slug: jobsnormalize-get
      parameters:
      - in: query
        name: job_title
        description: Find the canonical job title(s) for jobs matching the given text
          fragment
      - in: query
        name: limit
        description: Maximumn number of job title synonyms to return
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Normalization
---