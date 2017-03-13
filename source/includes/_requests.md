# Requests

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
  "batchId": "",
  "packageCode": ""
  }
]
```

The PAWS API requires all requests to:

- Be made as type `POST`.
- Include your `userName`, `password`, and `apiKey` in the request body data.
- ...later add info about encrypting field level junk...

### Full Parameter List

<aside class="notice">
You can refer to an API's specific documentation for details of what parameters it uses and if they are required or optional, as well as their format restrictions.
</aside>

Parameter | Description 
--------- | ------------
`member`  | The object that contains all member related information for a request.
`memberUserId' | Used to set the member's user Id for online credit services.
`memberPassword` | Used to set the member's password for online credit services. 
`membershipNumber` | The unique identifier for this member.
`firstName` | The member's first name.
`middleName` | The member's middle initial.
`lastName` | The member's last name.
`suffix` | The generation of the member.
`dateOfBirth` | The member's date of birth.
`ssn` | The member's Social Security Number or Social Insurance Number.
`emailAddress` | The member's email address.
`phoneNumber` | The member's phone number.
`address1` | The member's primary address.
`address2` | The member's secondary address.
`address3` | Additional address for the member.
`address4` | Additional address for the member.
`address5` | Additional address for the member.
`city` | The city for the member's primary address.
`stateOrProvince` | The state for the member's primary address.
`postalCode` | The postal code for the member's primary address.
`customerServicePhoneNumber` | The ...
`batchId` | The unique Id of the activity batch collection.
'packageCode` | The unique code for the package.





