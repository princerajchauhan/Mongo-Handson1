==> "https://prepbytes-misc-images.s3.ap-south-1.amazonaws.com/assets/1640781204638-employee.json

    <!-- *********************** HANDSON 1 *************************** -->

Question.1 Create a database , give it name like ""Human_Resource"". Create a collection inside this named ""employee""
 ==> use Human_Resource

Question.2 Query the collection ""employee"" and list all the documents
 ==> db.employee.find()

 Questio.3 Query the collection ""employee"" and list the employees who are having salary more than 30000
  ==> db.employee.find({salary: {$gt: '30000'}})

Question.4 Query the collection ""employee"" and list the employees who are having experience more than 2 years.
 ==> db.employee.find({overallExp:{$gt: '2'}})

 Question.5 Query the collection ""employee"" and list the employees who are graduated after 2015 and having experience more than 1 year 
  ==> db.employee.find({yearGrad: {$gt: '2015'}, overallExp: {$gt: '1'}})

Question.6 Query the collection ""employee"" and update the salary of the employee whose salary is greater than 70000 to 65000.
 ==> db.employee.updateMany({salary: {$gt: '70000'}}, {$set: {salary: '65000'}})

 Question.7 Delete all the documents from ""employee"" where last company is Y"
  ==> db.employee.deleteMany({lastCompany: 'Y})