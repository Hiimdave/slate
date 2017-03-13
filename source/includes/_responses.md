# Responses

> Example response:

```json
[
  {
    "responseObject": "Success - Action succeeded.",
    "errorType": 200,
    "errorMessage": "",
    "emptyReport": "N",
    "developerMessage": ""
  }
]
```

All PAWS API responses will contain the following parameters:

Parameter | Description
--------- | -----------
`responseObject` | Contains the status and response type of the request.
`errorType` | The HTTP status code of the response.
`errorMessage` | The detailed error message for the response.
`emptyReport` | Signifies if the response is empty or not.
`developerMessage` | If any developer specific information can be given, the contents of that message will display here.

### Status Codes

The following status codes are used by the PAWS API for responses:

Status Code | Meaning
---------- | -------
200 | Success -- Your request was successfully made and processed.
400 | Bad Request -- Your request was invalid, malformed, or missing required data.
500 | Internal Server Error -- An error occured within our systems.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later.