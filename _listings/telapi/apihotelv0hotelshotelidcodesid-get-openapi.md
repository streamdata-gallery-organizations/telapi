---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Get all the details for a specific code available
    for the hotel.
  version: v0
  description: Read the details about a specific code available for the defined hotel.
host: api.hetras-certification.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels:
    get:
      summary: Get a list of all the hotels of a chain your application has access
        to.
      description: Get a list of all the hotels of a chain your application has access
        to..
      operationId: Hotels_GetHotels
      x-api-path-slug: apihotelv0hotels-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      responses:
        200:
          description: OK
      tags:
      - ""
      - Hotels
      - Of
      - Chain
      - Your
      - Application
      - Has
      - Access
      - To
  /api/hotel/v0/hotels/{hotelId}:
    get:
      summary: Get the details of the hotel with the speccified hotel id.
      description: Get the details of the hotel with the speccified hotel id..
      operationId: Hotels_GetHotel
      x-api-path-slug: apihotelv0hotelshotelid-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Hotel
      - Speccified
      - Hotel
      - Id
  /api/hotel/v0/hotels/{hotelId}/codes:
    get:
      summary: Get a list of codes for the specified hotel either filtered by type
        or code.
      description: "With this call you can find codes for a hotel by type or code.
        By default and without any filter criteria\r\n            defined it will
        return you all available codes."
      operationId: Codes_GetCodes
      x-api-path-slug: apihotelv0hotelshotelidcodes-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: code
        description: Return all codes matching the code
      - in: path
        name: hotelId
        description: The hotel id you are trying to find codes for
      - in: query
        name: type
        description: Return all codes available for the specified type
      responses:
        200:
          description: OK
      tags:
      - Codesthe
      - Specified
      - Hotel
      - Either
      - Filtered
      - By
      - Type
      - Code
  /api/hotel/v0/hotels/{hotelId}/codes/{id}:
    get:
      summary: Get all the details for a specific code available for the hotel.
      description: Read the details about a specific code available for the defined
        hotel.
      operationId: Codes_GetCode
      x-api-path-slug: apihotelv0hotelshotelidcodesid-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the code available for
      - in: path
        name: id
        description: The code identifier you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Code
      - Availablethe
      - Hotel
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