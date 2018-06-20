---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Get the count of all rooms in the hotel matching
    the given filter criteria.
  version: v0
  description: Get the count of all rooms in the hotel matching the given filter criteria..
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
  /api/hotel/v0/hotels/{hotelId}/rateplans/$count:
    get:
      summary: Get the count of all rateplans in the hotel matching the given filter
        criteria.
      description: Get the count of all rateplans in the hotel matching the given
        filter criteria..
      operationId: RatePlans_GetRateplansCount
      x-api-path-slug: apihotelv0hotelshotelidrateplanscount-get
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
        description: The hotel you are counting the rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
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
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rateplans
      - In
      - Hotel
      - Matching
      - Given
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}:
    get:
      summary: Get all the details for a specific rateplan in the hotel.
      description: Read the details about a specific rateplan for the defined hotel.
      operationId: RatePlans_GetRateplan
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancode-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Rateplan
      - In
      - Hotel
  /api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates:
    get:
      summary: Get the setup of the daily rates for a specific rateplan and a defined
        timeperiod.
      description: "With this call you can read the daily rates setup including the
        cancellation policy and minimum guarantee per day for the\r\n            specified
        rateplan. You can specify a timeperiod to read the daily rates for. The rateplan
        needs to be active for at least\r\n            one business day in the defined
        time period and have rates loaded."
      operationId: RatePlans_GetRates
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancoderates-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: expand
        description: You can expand the supplements per room type on demand
      - in: query
        name: from
        description: Defines the last business day you would like to get rates for
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to see details for
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: to
        description: Defines the first business day you would like to get rates for
      - in: query
        name: top
        description: Amount of items to select
      responses:
        200:
          description: OK
      tags:
      - Setup
      - Of
      - Daily
      - Ratesa
      - Specific
      - Rateplan
      - Defined
      - Timeperiod
    patch:
      summary: Partially update a rate of the specified rateplan for the defined time
        period.
      description: "The hetras API is using this Patch Specification\r\n            to
        partially update an existing resource. Currently this call only allows to
        set the base price for non-derived rateplans if the rateplan\r\n            is
        active and already loaded for the specified time period.\r\n            \r\n
        \           A request example:\r\n            [\r\n              {\r\n                \"op\":
        \"replace\", \"path\": \"/base_price\", \"value\": 120.00\r\n              }\r\n
        \           ]\r\n            \r\n            For more details on how the API
        responds to errors please check our documentation on \r\n            Error
        Handling."
      operationId: RatePlans_PatchRates
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancoderates-patch
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: from
        description: Defines the last business day you would like to get rates for
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: body
        name: patchRequest
        description: A set of JSON Patch operations
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to update the daily rate details
          for
      - in: query
        name: to
        description: Defines the first business day you would like to get rates for
      responses:
        200:
          description: OK
      tags:
      - Partially
      - Update
      - Rate
      - Of
      - Specified
      - Rateplanthe
      - Defined
      - Time
      - Period
  /api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates/$count:
    get:
      summary: Get the count of all active and loaded daily rates for the defined
        rateplan in a specified time period.
      description: Get the count of all active and loaded daily rates for the defined
        rateplan in a specified time period..
      operationId: RatePlans_GetRatesCount
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancoderatescount-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: from
        description: Defines the last business day you would like to get rates for
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to count daily rates for
      - in: query
        name: to
        description: Defines the first business day you would like to get rates for
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Active
      - Loaded
      - Daily
      - Ratesthe
      - Defined
      - Rateplan
      - In
      - Specified
      - Time
      - Period
  /api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates/{businessDay}:
    get:
      summary: Get the setup of a daily rate for a specific business day and rateplan.
      description: Read the setup of the daily rate for the defined rateplan for that
        specific business day.
      operationId: RatePlans_GetRate
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancoderatesbusinessday-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: businessDay
        description: The business day you want to get the rate setup for
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to see details for
      responses:
        200:
          description: OK
      tags:
      - Setup
      - Of
      - Daily
      - Ratea
      - Specific
      - Business
      - Day
      - Rateplan
    patch:
      summary: Partially update a rate of the specified rateplan for a defined business
        day.
      description: "The hetras API is using this Patch Specification\r\n            to
        partially update an existing resource. Currently this call only allows to
        set the base price for non-derived rateplans if the rateplan\r\n            is
        active and already loaded for the specified business day.\r\n            \r\n
        \           A request example:\r\n            [\r\n              {\r\n                \"op\":
        \"replace\", \"path\": \"/base_price\", \"value\": 120.00\r\n              }\r\n
        \           ]\r\n            \r\n            For more details on how the API
        responds to errors please check our documentation on \r\n            Error
        Handling."
      operationId: RatePlans_PatchRate
      x-api-path-slug: apihotelv0hotelshotelidrateplansrateplancoderatesbusinessday-patch
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: businessDay
        description: The business day of the daily rate you want to update
      - in: path
        name: hotelId
        description: The hotel id the rateplan belongs to
      - in: body
        name: patchRequest
        description: A set of JSON Patch operations
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: rateplanCode
        description: The code of the rateplan you want to update the daily rate details
          for
      responses:
        200:
          description: OK
      tags:
      - Partially
      - Update
      - Rate
      - Of
      - Specified
      - Rateplana
      - Defined
      - Business
      - Day
  /api/hotel/v0/hotels/{hotelId}/room_types:
    get:
      summary: Get a list with the details of all room types for for the specified
        hotel id.
      description: With this call you can load the details about a all available room
        types for the specified hotel.
      operationId: RoomTypes_GetRoomTypes
      x-api-path-slug: apihotelv0hotelshotelidroom-types-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - ""
      - Room
      - Typesfor
      - Specified
      - Hotel
      - Id
  /api/hotel/v0/hotels/{hotelId}/room_types/{code}:
    get:
      summary: Get all the details for a specific room type in the hotel.
      description: With this call you can load the details about a specific room type
        in the hotel.
      operationId: RoomTypes_GetRoomType
      x-api-path-slug: apihotelv0hotelshotelidroom-typescode-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: code
        description: The code of the room type you want to see details for
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Room
      - Type
      - In
      - Hotel
  /api/hotel/v0/hotels/{hotelId}/rooms:
    get:
      summary: Get a list of rooms using the provided filtering and pagination criteria.
      description: "Find all rooms for the hotel that match the specified filter criteria.
        The filtering will be done based on the current state of\r\n            the
        rooms."
      operationId: Rooms_GetRooms
      x-api-path-slug: apihotelv0hotelshotelidrooms-get
      parameters:
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: conditions
        description: Return results only for rooms that have the given room condition
          status
      - in: path
        name: hotelId
        description: The hotel you are trying to find rooms for
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: maintenances
        description: Return results only for rooms that have the given maintenance
          status
      - in: query
        name: occupancy
        description: Return results only for rooms that have the given frontdesk ocuppancy
          status
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: top
        description: Amount of items to select
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Using
      - Provided
      - Filtering
      - Pagination
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rooms/$count:
    get:
      summary: Get the count of all rooms in the hotel matching the given filter criteria.
      description: Get the count of all rooms in the hotel matching the given filter
        criteria..
      operationId: Rooms_GetRoomsCount
      x-api-path-slug: apihotelv0hotelshotelidroomscount-get
      parameters:
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: conditions
        description: Return results only for rooms that have the given room condition
          status
      - in: path
        name: hotelId
        description: The hotel you are counting the rooms for
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: maintenances
        description: Return results only for rooms that have the given maintenance
          status
      - in: query
        name: occupancy
        description: Return results only for rooms that have the given frontdesk ocuppancy
          status
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rooms
      - In
      - Hotel
      - Matching
      - Given
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