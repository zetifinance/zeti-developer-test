# Zeti's Developer Test
 
Thanks for taking the time to do this test and apply to work at Zeti. This test should not take  you more than 2 hours - if you find yourself taking longer than this, please just stop work and take down any notes about where you wanted to take the work if you had time. This test is not language specific, however the test should be taken in whatever language has been specified by your recruitment contact. If you have any questions, please get in touch either through an issue on this repository or via email to hello@zeti.co.uk or your usual contact. Submissions should be done by sending a link to your own (private) GitHub repo to your recruitment contact, or however they have asked you to do it. If you are sending over a private GitHub repository, please makesure to add danbasszeti to the users allowed to see the repository. Please don't fork this repo to submit.

## The Task

Bill a customer for the usage of their fleet of 2 vehicles.

The customer (Asset Operator) is called Bob's Taxis. They have a fleet of 2 vehicles (number plates CBDH 789 and 86532 AZE), and pay £0.207 per mile they travel.  They're happy to receive this bill in a variety of formats such as JSON, CSV, PDF, HTML, XML etc - you can choose whichever suits you best. There is a very limited telematics providers API to help you here: https://funczetiinterviewtest.azurewebsites.net/api/swagger/ui

Write a program that queries the API at runtime and then displays how much Bob's taxi's owes for the mileage they covered between 2021-02-01T00:00:00Z and 2021-02-28T23:59:00Z. This can be a console app with those parameters hardcoded (so long as the API response is not hardcoded) writing out to a file, or it can be something more sophisticated like a React or ASP.NET app that displays the results in the browser - please include any instructions for running more sophisticated solutions in a readme.md in your repository root (i.e. if your ASP.NET based solution takes query parameters, include the example URL to make it quicker and easier for the Zeti employee to evaluate your test).

Include at least one test of what you feel is the most important part of the core logic of the application.

### Tips
Mileage readings come from devices called odometers. These always provide the total number of miles the vehicle has travelled until this point in time. So to work out how many miles a vehicle has covered between two times, you'd need to subtract the earlier reading from the later one (as it is not possible to cover negative miles). For example, if you checked a vehicle's odometer on monday and it read 30,000 miles, and then checked it the following monday and it read 35,000 miles, then the vehicle would have covered 5000 miles in that week. 

To turn mileage readings into bills, we use a cost-per-mile. So in the above example of a vehicle that covered 5000 miles, if that vehicle's cost-per-mile was £0.10 then the operator would be charged £500. 
### Things to consider

- Make it work, Make it right, Make it fast. Don't get hung up on design before you have a working implementation - this is a short test.
- Consider what the best long term identifier for a vehicle is.
- Testing
- Design Patterns, what fits this problem best?
