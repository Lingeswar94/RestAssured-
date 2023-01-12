# RestAssured-
THis topic is covered by RestAssured concept 


Json :

Standalone JsonPath (included if you depend on the rest-assured artifact). Makes it easy to parse JSON documents. Note that this JsonPath implementation uses Groovy's GPath syntax and is not to be confused with Kalle Stenflo's JsonPath implementation. 

https://jsonpath.curiousconcept.com/#

http://jsonviewer.stack.hu/

JSon Path Expression :

{
"Employees" : [
{
"userId":"Lingesh",
"jobTitleName":"Developer",
"firstName":"Romin",
"lastName":"Irani",
"preferredFullName":"Romin Irani",
"employeeCode":"E1",
"region":"CA",
"phoneNumber":"408-1234567",
"emailAddress":"romin.k.irani@gmail.com"
},
{
"userId":"Tamil",
"jobTitleName":"Developer",
"firstName":"Neil",
"lastName":"Irani",
"preferredFullName":"Neil Irani",
"employeeCode":"E2",
"region":"CA",
"phoneNumber":"408-1111111",
"emailAddress":"neilrirani@gmail.com"
},
{
"userId":"Pradeep",
"jobTitleName":"Program Directory",
"firstName":"Tom",
"lastName":"Hanks",
"preferredFullName":"Tom Hanks",
"employeeCode":"E3",
"region":"CA",
"phoneNumber":"408-2222222",
"emailAddress":"tomhanks@gmail.com"
}
]
}


Method Path:

1. $..userId ----  all user id from file .
2. $.Employees[*].userId----  another method all user id from file .
3. $.Employees.[2].jobTitleName---taken second emplyoo job tile 
4. $.Employees[2].userId----  taken second emply  all details 
5. $.Employees.[0,1]---- taken detail for 0 and 1 
6. $.Employees.[1:] ----  taken emplpee starting from  1 and till end .
7. $.Employees.[-1:] ----  taken emplpee last 
8. $.Employees[?(@.phoneNumber)]----indentfy which Employees have phnoe number  .
9. $.Employees[?(@.jobTitleName="Developer")]-----which indenfy get jobtitle 
10. $.Employees[?(@.employeeCode>10)]  ---validate to employee greater than 10.
11. $.Employees[?(@.employeeCode>10)]
12. $.Employees[?(@.employeeCode>15)]
13. $.Employees[-1,-2]  
