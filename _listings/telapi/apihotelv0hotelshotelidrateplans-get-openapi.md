---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Get a list of rateplans for the specified hotel
    id matching the filter criteria.
  version: v0
  description: "With this call you can find rateplans for a hotel by different filters.
    By default and without any filter criteria\r\n            defined it will return
    you all active rateplans."
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
  /api/hotel/v0/hotels/{hotelId}/rateplans:
    get:
      summary: Get a list of rateplans for the specified hotel id matching the filter
        criteria.
      description: "With this call you can find rateplans for a hotel by different
        filters. By default and without any filter criteria\r\n            defined
        it will return you all active rateplans."
      operationId: RatePlans_GetRateplans
      x-api-path-slug: apihotelv0hotelshotelidrateplans-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: baseRateplan
        description: Return all rateplans having the specified rateplan as base rateplan
      - in: query
        name: channelCode
        description: Return all rateplans sold through the specified channel
      - in: query
        name: channelGroup
        description: Return all rateplans that are sold through at least one channel
          out of the specified channel group
      - in: query
        name: commissionable
        description: Return all rateplans having commisionable status
      - in: query
        name: group
        description: Return all rateplans belonging to the specified rateplan group
      - in: path
        name: hotelId
        description: The hotel id you are trying to find rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: marketCodes
        description: Return all rateplans having one of the specified values as a
          market code
      - in: query
        name: roomTypes
        description: Return all rateplans by which at least one of the specified room
          types are sold
      - in: query
        name: sellingStatus
        description: Specify which rateplans to return
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: top
        description: Amount of items to select
      responses:
        200:
          description: OK
      tags:
      - Rateplansthe
      - Specified
      - Hotel
      - Id
      - Matching
      - Filter
      - Criteria
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