# API List

## Enroll

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": "",
    "firstName": "",
    "middleName": "",
    "lastName": "",
    "suffix": "",
    "dateOfBirth": "",
    "ssn": "",
    "emailAddress": "",
    "phoneNumber": "",
    "address1": "",
    "address2": "",
    "address3": "",
    "address4": "",
    "address5": "",
    "city": "",
    "stateOrProvince": "",
    "postalCode": "",
    "customerServicePhoneNumber": ""
    },
  "packageCode": ""
  }
]
```

The Enroll API enrolls a member into the specified package with Kroll.

**Parameters:**

Name | Required | Formatting
---- | -------- | -------
`membershipNumber` | Yes | Must be alphanumeric, between 1 and 12 characters, and without spaces.
`firstName` | Yes | Must be alphabetic and between 1 and 50 characters.
`middleName` | No | Must be alphabetic and exactly 1 character.
`lastName` | Yes | Must be alphabetic and between 1 and 50 characters.
`suffix` | No | Must be one of the following: Jr, Sr, I-IX
`dateOfBirth` | No | Must be in `mm/DD/yyyy` format.
`ssn` | No | Must be exactly 9 numeric characters.
`emailAddress` | No | Must match a valid email syntax.
`phoneNumber` | No | Must be exactly 10 numeric characters.
`address1` | Yes | Must be alphanumeric and between 1 and 100 characters.
`address2` | No | See above.
`address3` | No | See above.
`address4` | No | See above.
`address5` | No | See above.
`city` | Yes | Must be alphabetic and between 1 and 70 characters.
`stateProvince` | Yes | Must be a valid 2 character US state or CA province abbreviation.
`postalCode` | Yes | Must be a valid US post code and be exactly 5 or 9 characters, or a valid CA post code in `L#L #L#` format and be exactly 7 characters including the space.
`customerServicePhoneNumber` | No | Must be exactly 10 numeric characters.
`packageCode` | Yes | Must be a valid, 3 character Kroll package code that is associated to your client. 



## Enroll and Load

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "memberUserId": "",
    "memberPassword": "",
    "membershipNumber": "",
    "firstName": "",
    "middleName": "",
    "lastName": "",
    "suffix": "",
    "dateOfBirth": "",
    "ssn": "",
    "emailAddress": "",
    "phoneNumber": "",
    "address1": "",
    "address2": "",
    "address3": "",
    "address4": "",
    "address5": "",
    "city": "",
    "stateOrProvince": "",
    "postalCode": "",
    "customerServicePhoneNumber": ""
    },
  "packageCode": ""
  }
]
```

<aside class="notice">
You can only call Enroll And Load if you are configured with Online Credit Services.
</aside>

The Enroll and Load API enrolls a member into the specified package with Kroll and enrolls them in online credit services with the requested username and password.

**Parameters:**

Name | Required | Format
---- | -------- | -------
`memberUserId` | Yes | Must be ...
`memberPassword` | Yes | Must be ...
`membershipNumber` | Yes | Must be alphanumeric, between 1 and 12 characters, and without spaces.
`firstName` | Yes | Must be alphabetic and between 1 and 50 characters.
`middleName` | No | Must be alphabetic and exactly 1 character.
`lastName` | Yes | Must be alphabetic and between 1 and 50 characters.
`suffix` | No | Must be one of the following: Jr, Sr, I-IX
`dateOfBirth` | Yes | Must be in `mm/DD/yyyy` format.
`ssn` | No | Must be exactly 9 numeric characters.
`emailAddress` | Yes | Must match a valid email syntax.
`phoneNumber` | No | Must be exactly 10 numeric characters.
`address1` | Yes | Must be alphanumeric and between 1 and 100 characters.
`address2` | No | See above.
`address3` | No | See above.
`address4` | No | See above.
`address5` | No | See above.
`city` | Yes | Must be alphabetic and between 1 and 70 characters.
`stateProvince` | Yes | Must be a valid 2 character US state or CA province abbreviation.
`postalCode` | Yes | Must be a valid US post code and be exactly 5 or 9 characters, or a valid CA post code in `L#L #L#` format and be exactly 7 characters including the space.
`customerServicePhoneNumber` | No | Must be exactly 10 numeric characters.
`packageCode` | Yes | Must be a valid, 3 character Kroll package code that is associated to your client. 


## Cancel

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": ""
    }
  }
]
```

The Cancel API cancels an active member's services with Kroll.  

**Parameters:**

Name | Required | Format
---- | -------- | -------
`membershipNumber` | Yes | Must match an existing Active member enrolled in a package associated to your client.


## Reactivate

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": "",
    "firstName": "",
    "middleName": "",
    "lastName": "",
    "suffix": "",
    "dateOfBirth": "",
    "ssn": "",
    "emailAddress": "",
    "phoneNumber": "",
    "address1": "",
    "address2": "",
    "address3": "",
    "address4": "",
    "address5": "",
    "city": "",
    "stateOrProvince": "",
    "postalCode": "",
    "customerServicePhoneNumber": ""
    },
  "packageCode": ""
  }
]
```

The Reactivate API reinstates a cancelled member's services with Kroll.

**Parameters:**

Name | Required | Format
---- | -------- | -------
`membershipNumber` | Yes | Must match an existing Active member enrolled in a package associated to your client.


## Update Demographics

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": "",
    "firstName": "",
    "middleName": "",
    "lastName": "",
    "suffix": "",
    "dateOfBirth": "",
    "ssn": "",
    "emailAddress": "",
    "phoneNumber": "",
    "address1": "",
    "address2": "",
    "address3": "",
    "address4": "",
    "address5": "",
    "city": "",
    "stateOrProvince": "",
    "postalCode": "",
    "customerServicePhoneNumber": ""
    }
  }
]
```

Description of the API goes here

**Parameters:**

Name | Required | Format
---- | -------- | -------
Example | Yes | `mmDDyyyy`



## Reorder Credit Auth

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": ""
    }
  }
]
```

Description of the API goes here

**Parameters:**

Name | Required | Format
---- | -------- | -------
Example | Yes | `mmDDyyyy`



## Reorder Membership Card

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": ""
    }
  }
]
```

Description of the API goes here

**Parameters:**

Name | Required | Format
---- | -------- | -------
Example | Yes | `mmDDyyyy`



## Reorder Membership Packet

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "member": {
    "membershipNumber": ""
    }
  }
]
```

Description of the API goes here

**Parameters:**

Name | Required | Format
---- | -------- | -------
Example | Yes | `mmDDyyyy`



## Get Batch List

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": ""
  }
]
```

The Get Batch List API returns a listing of all Activity Batches in the Kroll system for your members that have not been confirmed yet.

**Parameters:**

No API specific parameters are required.



## Get Batch

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "batchId": ""
  }
]
```

The Get Batch API will return the collection of Activity data for members in the Kroll system contained within the specified batch.

**Parameters:**

Name | Required | Format
---- | -------- | -------
`batchId` | Yes | Must be an alphanumeric string for a valid Batch.




## Confirm Batch

> Example request:

```json
[
  {
  "apiKey": "",
  "userName": "",
  "password": "",
  "batchId": ""
  }
]
```

The Confirm Batch API updates a specified Activity Batch to the "Confirmed" status, which will remove it from the available batches seen in the Get Batch List call to update.

**Parameters:**

Name | Required | Format
---- | -------- | -------
`batchId` | Yes | Must be an alphanumeric string for a valid Batch.


