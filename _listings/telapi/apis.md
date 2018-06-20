---
name: TelAPI
x-slug: telapi
description: Zang offers business communications tools & voice app development platforms
  that bring innovation and ease to unified communications & collaboration solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
x-kinRank: "9"
x-alexaRank: "1071695"
tags: TelAPI
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apis.md
specificationVersion: "0.14"
apis:
- name: hetras Hotel API Version 0 Get a list of all the hotels of a chain your application
    has access to.
  x-api-slug: hetras-hotel-api-version-0
  description: Get a list of all the hotels of a chain your application has access
    to..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels
  tags: ',Hotels,Of,Chain,Your,Application,Has,Access,To'
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotels-get-openapi.md
- name: hetras Hotel API Version 0 Get the details of the hotel with the speccified
    hotel id.
  x-api-slug: hetras-hotel-api-version-0
  description: Get the details of the hotel with the speccified hotel id..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}
  tags: Details,Of,Hotel,Speccified,Hotel,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelid-get-openapi.md
- name: hetras Hotel API Version 0 Get a list of codes for the specified hotel either
    filtered by type or code.
  x-api-slug: hetras-hotel-api-version-0
  description: "With this call you can find codes for a hotel by type or code. By
    default and without any filter criteria\r\n            defined it will return
    you all available codes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/codes
  tags: Codesthe,Specified,Hotel,Either,Filtered,By,Type,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidcodes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidcodes-get-openapi.md
- name: hetras Hotel API Version 0 Get all the details for a specific code available
    for the hotel.
  x-api-slug: hetras-hotel-api-version-0
  description: Read the details about a specific code available for the defined hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/codes/{id}
  tags: Detailsa,Specific,Code,Availablethe,Hotel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidcodesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidcodesid-get-openapi.md
- name: hetras Hotel API Version 0 Get a list of rateplans for the specified hotel
    id matching the filter criteria.
  x-api-slug: hetras-hotel-api-version-0
  description: "With this call you can find rateplans for a hotel by different filters.
    By default and without any filter criteria\r\n            defined it will return
    you all active rateplans."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans
  tags: Rateplansthe,Specified,Hotel,Id,Matching,Filter,Criteria
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplans-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplans-get-openapi.md
- name: hetras Hotel API Version 0 Get the count of all rateplans in the hotel matching
    the given filter criteria.
  x-api-slug: hetras-hotel-api-version-0
  description: Get the count of all rateplans in the hotel matching the given filter
    criteria..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/$count
  tags: Count,Of,,Rateplans,In,Hotel,Matching,Given,Filter,Criteria
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplanscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplanscount-get-openapi.md
- name: hetras Hotel API Version 0 Get all the details for a specific rateplan in
    the hotel.
  x-api-slug: hetras-hotel-api-version-0
  description: Read the details about a specific rateplan for the defined hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}
  tags: Detailsa,Specific,Rateplan,In,Hotel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancode-get-openapi.md
- name: hetras Hotel API Version 0 Get the setup of the daily rates for a specific
    rateplan and a defined timeperiod.
  x-api-slug: hetras-hotel-api-version-0
  description: "With this call you can read the daily rates setup including the cancellation
    policy and minimum guarantee per day for the\r\n            specified rateplan.
    You can specify a timeperiod to read the daily rates for. The rateplan needs to
    be active for at least\r\n            one business day in the defined time period
    and have rates loaded."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates
  tags: Setup,Of,Daily,Ratesa,Specific,Rateplan,Defined,Timeperiod
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderates-get-openapi.md
- name: hetras Hotel API Version 0 Partially update a rate of the specified rateplan
    for the defined time period.
  x-api-slug: hetras-hotel-api-version-0
  description: "The hetras API is using this Patch Specification\r\n            to
    partially update an existing resource. Currently this call only allows to set
    the base price for non-derived rateplans if the rateplan\r\n            is active
    and already loaded for the specified time period.\r\n            \r\n            A
    request example:\r\n            [\r\n              {\r\n                \"op\":
    \"replace\", \"path\": \"/base_price\", \"value\": 120.00\r\n              }\r\n
    \           ]\r\n            \r\n            For more details on how the API responds
    to errors please check our documentation on \r\n            Error Handling."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates
  tags: Partially,Update,Rate,Of,Specified,Rateplanthe,Defined,Time,Period
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderates-patch-openapi.md
- name: hetras Hotel API Version 0 Get the count of all active and loaded daily rates
    for the defined rateplan in a specified time period.
  x-api-slug: hetras-hotel-api-version-0
  description: Get the count of all active and loaded daily rates for the defined
    rateplan in a specified time period..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates/$count
  tags: Count,Of,,Active,Loaded,Daily,Ratesthe,Defined,Rateplan,In,Specified,Time,Period
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderatescount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderatescount-get-openapi.md
- name: hetras Hotel API Version 0 Get the setup of a daily rate for a specific business
    day and rateplan.
  x-api-slug: hetras-hotel-api-version-0
  description: Read the setup of the daily rate for the defined rateplan for that
    specific business day.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates/{businessDay}
  tags: Setup,Of,Daily,Ratea,Specific,Business,Day,Rateplan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderatesbusinessday-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderatesbusinessday-get-openapi.md
- name: hetras Hotel API Version 0 Partially update a rate of the specified rateplan
    for a defined business day.
  x-api-slug: hetras-hotel-api-version-0
  description: "The hetras API is using this Patch Specification\r\n            to
    partially update an existing resource. Currently this call only allows to set
    the base price for non-derived rateplans if the rateplan\r\n            is active
    and already loaded for the specified business day.\r\n            \r\n            A
    request example:\r\n            [\r\n              {\r\n                \"op\":
    \"replace\", \"path\": \"/base_price\", \"value\": 120.00\r\n              }\r\n
    \           ]\r\n            \r\n            For more details on how the API responds
    to errors please check our documentation on \r\n            Error Handling."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rateplans/{rateplanCode}/rates/{businessDay}
  tags: Partially,Update,Rate,Of,Specified,Rateplana,Defined,Business,Day
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrateplansrateplancoderatesbusinessday-patch-openapi.md
- name: hetras Hotel API Version 0 Get a list with the details of all room types for
    for the specified hotel id.
  x-api-slug: hetras-hotel-api-version-0
  description: With this call you can load the details about a all available room
    types for the specified hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/room_types
  tags: List,Details,Of,,Room,Typesfor,Specified,Hotel,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroom-types-get-openapi.md
- name: hetras Hotel API Version 0 Get all the details for a specific room type in
    the hotel.
  x-api-slug: hetras-hotel-api-version-0
  description: With this call you can load the details about a specific room type
    in the hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/room_types/{code}
  tags: Detailsa,Specific,Room,Type,In,Hotel
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroom-typescode-get-openapi.md
- name: hetras Hotel API Version 0 Get a list of rooms using the provided filtering
    and pagination criteria.
  x-api-slug: hetras-hotel-api-version-0
  description: "Find all rooms for the hotel that match the specified filter criteria.
    The filtering will be done based on the current state of\r\n            the rooms."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rooms
  tags: Rooms,Using,Provided,Filtering,Pagination,Criteria
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidrooms-get-openapi.md
- name: hetras Hotel API Version 0 Get the count of all rooms in the hotel matching
    the given filter criteria.
  x-api-slug: hetras-hotel-api-version-0
  description: Get the count of all rooms in the hotel matching the given filter criteria..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rooms/$count
  tags: Count,Of,,Rooms,In,Hotel,Matching,Given,Filter,Criteria
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroomscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroomscount-get-openapi.md
- name: hetras Hotel API Version 0 Request available rooms using a given criteria.
  x-api-slug: hetras-hotel-api-version-0
  description: Request available rooms using a given criteria..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rooms/available
  tags: Request,Available,Rooms,Using,Given,Criteria
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroomsavailable-get-openapi.md
- name: hetras Hotel API Version 0 Get all the details for a specific room in the
    hotel.
  x-api-slug: hetras-hotel-api-version-0
  description: With this call you can load the details about a specific room in the
    hotel. It will show you the current status of the room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rooms/{roomNumber}
  tags: Detailsa,Specific,Room,In,Hotel
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroomsroomnumber-get-openapi.md
- name: hetras Hotel API Version 0 Partially updates a room.
  x-api-slug: hetras-hotel-api-version-0
  description: "The hetras API is using this Patch Specification\r\n            to
    partially update an existing resource. Currently this call only allows to modify
    condition and housekeeping occupancy status of the room.\r\n            \r\n            A
    request example:\r\n            [\r\n              {\r\n                \"op\":
    \"replace\", \"path\": \"/status/condition\", \"value\": \"CleanNotInspected\"\r\n
    \             }, {\r\n                \"op\": \"replace\", \"path\": \"/status/housekeeping_occupancy\",
    \"value\": \"Vacant\"\r\n              }\r\n            ]\r\n            \r\n
    \           For more details on how the API responds to errors please check our
    documentation on \r\n            Error Handling."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net////api/hotel/v0/hotels/{hotelId}/rooms/{roomNumber}
  tags: Partially,Updates,Room
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/apihotelv0hotelshotelidroomsroomnumber-patch-openapi.md
- name: hetras Hotel API Version 0
  x-api-slug: hetras-hotel-api-version-0
  description: Zang offers business communications tools & voice app development platforms
    that bring innovation and ease to unified communications & collaboration solutions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net//
  tags: TelAPI
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/telapi/master/_listings/telapi/openapi.md
x-common:
- type: x-base
  url: https://api.telapi.com
- type: x-blog
  url: http://www.TelAPI.com/blog/
- type: x-blog-rss
  url: http://www.telapi.com/blog/feed/
- type: x-contact-form
  url: http://www.telapi.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/telapi
- type: x-crunchbase
  url: https://crunchbase.com/organization/zang-io
- type: x-developer
  url: http://www.telapi.com/docs/
- type: x-email
  url: support@telapi.com
- type: x-github
  url: https://github.com/TelAPI
- type: x-pricing
  url: http://www.telapi.com/pricing
- type: x-privacy
  url: https://www.telapi.com/legal/privacy-policy
- type: x-selfservice-registration
  url: https://www.telapi.com/signup
- type: x-status
  url: http://status.telapi.com/
- type: x-terms-of-service
  url: https://www.telapi.com/legal/tos
- type: x-twitter
  url: https://twitter.com/TelAPI
- type: x-twitter
  url: https://twitter.com/Zang_io
- type: x-website
  url: http://www.telapi.com
- type: x-website
  url: http://telapi.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---