## Learning Employees
[Object attributes](#objects)  
[Data mapping]()  
[API endpoints]()  
[API example]()  
  
The object employee contains all personal and employment details of an employee.

### Object attributes {#objects}
An employee is a person with one or more employments.  
![](learning_attributes.png)  
  
Attributes person details  
| **Attribute**           | **Description**|
| ------------------------| ---------------|
| `personId`              | Unique id for the Person row within the tenant                           |
| `personCode`            | The logical person code of the employee                                  |
| `Initials`              | The initials of the employee.                                            |
| `firstNames`            | The official given names of the employee as stored in the HR Core system |
| `KnowAs`                | The name which is used by the employee as his first name                 |
| `lastNameAtBirth`       | The last name at birth of the employee. Also known as the family name    |
| `lastNameAtBirthPrefix` | The prefix of the last name at birth                                     |
| `lastName`              | The last which is currently used  by the employee as his last name       |
| `lastNamePrefix`        | The prefix of the last name as used currently                            |
| `nameAssembleOrder`     | Code of the assemble order that the core system uses for the last name. The assembly order is depending on the core system and the logic behind it.|
| `partnerName`           | The partner last name                                                    |
| `partnerNamePrefix`     | The prefix of the partner last name                                      |
| `titlePrefix`           | The formal title which will be used as a prefix before the name like Doctor, Professor, et cetera |
| `titleSuffix`           | The formal title which will be used as postfix after the name like MSc or Master of Science       |
| `gender`                | Gender of the person.<br>Supported values are Male / Female.<br>_Note: other type of genders will be shown as Not Known_ |
| `birthDate`             | Date of birth                                                            |
| `deceased`              | Indicated if the employee deceased                                       |
| `UserUID`               | Digital Identity of the user from the portal                             |
| `emailAddresses` <ul><li>type</li><li>address</li></ul> | List of the addresses of the employee. <br>The fields are: <ul><li>type like Business, Private, et cetera</li><li>address</li></ul>|
| `Addresses` <ul><li>type</li><li>street</li><li>houseNumber</li><li>houseNumberAdditional</li><li>locationDesignation</li><li>postalCode</li><li>city</li><li>region</li><li>country</li></ul>| List of the addresses of the employee. <br>The fields are:<ul><li>type like Home, Post, et cetera</li><li>street name</li><li>house number</li><li>house number additional</li><li>Location designation</li><li>Postal code</li><li>City</li><li>Region</li><li>Country code</li></ul> |
| `phoneNumbers`<ul><li>type</li><li>number</li></ul>  | list of phone numbers of the employee <ul><li>type like Business, Home, Mobile, et cetera</li><li>number</li></ul>|


