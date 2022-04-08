#Abercrombie AEM Developer Skill Assessment
1. Clone this repository.
2. Complete exercises below by creating/modifying code. You can architect the project how you like re: folder structure, how you name your files, etc. Use your best judgement as a developer.
3. Push the code to your own public Git repository, and send the link to your recruiter / rep.
4. Pretend your code is going into a `PRODUCTION` environment, or that you are writing a pull request for an established open source project. Do not rush these exercises or cut corners in the name of speed. We aren't interested in the code you can write under pressure; no one writes amazing code when they are rushing. This is your chance to show off. Write your best code.
5. This exercise is to be completed without coaching or other outside assistance. Obviously, you may feel free to use whatever online resources you like -- `StackOverflow` etc -- but it is not acceptable to utilize other developers to help you finish this task.

##Exercise 1:

A form has the following fields: First Name, Last Name, Age, Country and a Submit button. A validation check is done when the user enters details and clicks on submit button. For the validation, fetch the node details /etc/age, having min and max age. If the user entered age lies in between the min and max value, all the user details will be saved inside JCR (under `/var/anf-code-challenge`) otherwise, an error message will be displayed with following text `You are not eligible`.

![](images/Exercise-1.png)

###Acceptance Criteria:
1. Fetch node details from /etc/age having properties: `minAge` and `maxAge`.
2. When submit button is clicked, validate the age and save the user details on a node under `/var/anf-code-challenge` after successful validation.
3. Populate the dialog dropdown (country component) dynamically using `JSON` in DAM.

###Note: 
1. Please deploy Exercise-1.zip onto your AEM 6.5.0
2. Please make use of skeleton code in `custombutton.js` to handle the submit button click and call `UserServlet.java` to perform the required validations.
