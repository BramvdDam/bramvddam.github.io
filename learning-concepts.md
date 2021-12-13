## Learning Concepts
[Pagination of the result set](#pagination)
[Delete a record](#delete)

### Pagination of the result set {#pagination}
To reduce the load of an endpoint each endpoint supports paging. If the results of an endpoint contain more than 500 records, the results set will end with a nextLink tag. The nextLink indicates that there are more pages to load. If there is no nextLink at the end of the page, it means that it’s the last page of the result set. The default value is 500 records, but it is possible to use less than that.

Example of nextLink in the Json results

An example of these versions is visible with a validFrom and validUntil
```
"value": [
{
"personCode": "T0011",
"initials": "J.",
"firstNames": "Jan",
"knownAs": "Jan",
"lastName": "Aalbers",
"lastNameAtBirth": "Aalbers",
"nameAssembleOrder": "1",
"gender": "Male",
"birthDate": "1956-06-07",
"phoneNumbers": [],
"emailAddresses": [],
"employments": [
{
"employmentCode": "1",
"hireDate": "2017-02-01",
"company": "001",
"employmentType": "1",
"jobProfile": "DEVELOPER",
"organizationUnit": "DEVELOPMENT",
"workingAmount": {
"amountOfWork": 20,
"unitOfWork": "Hours",
"periodOfWork": "Week"
}
}
"validFrom": "2017-02-01",
"validUntil": "2018-10-31"
},
{
"personCode": "T0011",
"initials": "J.",
"firstNames": "Jan",
"knownAs": "Jan",
"lastName": "Aalbers",
"lastNameAtBirth": "Aalbers",
"nameAssembleOrder": "1",
"gender": "Male",
"birthDate": "1956-06-07",
"phoneNumbers": [],
"emailAddresses": [],
"employments": [
{
"employmentCode": "1",
"hireDate": "2017-02-01",
"company": "001",
"employmentType": "1",
"jobProfile": "DEVELOPER",
"organizationUnit": "DEVELOPMENT",
"workingAmount": {
"amountOfWork": 32,
"unitOfWork": "Hours",
"periodOfWork": "Week"
}
}
"validFrom": "2018-11-01",
"validUntil": "2019-03-31"
},
{
"personCode": "T0011",
"initials": "J.",
"firstNames": "Jan",
"knownAs": "Jan",
"lastName": "Aalbers",
"lastNameAtBirth": "Aalbers",
"nameAssembleOrder": "1",
"gender": "Male",
"birthDate": "1956-06-07",
"phoneNumbers": [],
"emailAddresses": [],
"employments": [
{
"employmentCode": "1",
"hireDate": "2017-02-01",
"company": "001",
"employmentType": "1",
"jobProfile": "DESIGNER",
"organizationUnit": "UX",
"workingAmount": {
"amountOfWork": 32,
"unitOfWork": "Hours",
"periodOfWork": "Week"
}
}
"validFrom": "2019-04-01",
"validUntil": "9999-12-31"
}
]
}]]>
```

### Delete a record {#delete}
After a record is deleted in the core system, the API will return the record with his id and the flag isDelete = true.

This delete means that the whole record including all version are delete.

For example
```
"id": "907624",
"isDeleted": true,
"shortName": "907624"
} ]]>
```
