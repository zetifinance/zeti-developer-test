# Zeti's Backend Developer Test
 
Thanks for taking the time to do this test and apply to work at Zeti. This test should not take  you more than 2 hours - if you find yourself taking longer than this, please just stop work and take down any notes about where you wanted to take the work if you had time. This test is not language specific, however the test should be taken in whatever language has been specified by your recruitment contact. If you have any questions, please get in touch either through an issue on this repository or via email to hello@zeti.co.uk or your usual contact. Submissions should be done by sending a link to your own GitHub repo to your recruitment contact, or however they have asked you to do it. Please don't fork this repo to submit.

## The Task

Bill a customer for the usage of their fleet of 2 vehicles.

The customer (Asset Operator) is called Bob's Taxis has a fleet of 2 vehicles (number plates CBDH 789 and 86532 AZE), and pays £0.207 per mile they travel. This means that if one vehicle travelled 50 miles and the other vehicle travelled 150 miles, overall they would be billed 200 miles multiplied by £0.207 which would £41.40. They're happy to receive this bill in a variety of formats such as JSON, CSV, PDF, HTML, XML etc - you can choose whichever suits you best. There is a very limited telematics providers API to help you here: https://funczetiinterviewtest.azurewebsites.net/api/swagger/ui

Write a program that queries the API and then creates a bill file for the mileage they covered between 2021-02-01T00:00:00Z and 2021-02-28T23:59:00Z.

### Things to consider

- Make it work, Make it right, Make it fast. Don't get hung up on design before you have a working implementation - this is a short test.
- Consider what the best long term identifier for a vehicle is.
- Design Patterns
- Testing