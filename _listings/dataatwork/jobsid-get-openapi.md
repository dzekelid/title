---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Job Title and Description
  description: Retrieves the name, description, and UUID of a job by specifying its
    O*NET SOC Code or UUID.
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