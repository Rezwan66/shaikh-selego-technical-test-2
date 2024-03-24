# Technical test

## Introduction

Fabien just came back from a meeting with an incubator and told them we have a platform “up and running” to monitor people's activities and control the budget for their startups !

All others developers are busy and we need you to deliver the app for tomorrow.
Some bugs are left and we need you to fix those. Don't spend to much time on it.

We need you to follow these steps to understand the app and to fix the bug :

- Sign up to the app
- Create at least 2 others users on people page ( not with signup )
- Edit these profiles and add aditional information
- Create a project
- Input some information about the project
- Input some activities to track your work in the good project

Then, see what happens in the app and fix the bug you found doing that.

## Then

Time to be creative, and efficient. Do what you think would be the best for your product under a short period.

### The goal is to fix at least 3 bugs and implement 1 quick win feature than could help us sell the platform

## Setup api

- cd api
- Run `npm i`
- Run `npm run dev`

## Setup app

- cd app
- Run `npm i`
- Run `npm run dev`

## Finally

Send us the project and answer to those simple questions :

- What bugs did you find ? How did you solve these and why ?
- Which feature did you develop and why ?
- Do you have any feedback about the code / architecture of the project and what was the difficulty you encountered while doing it ?

## Deliverables - Shaikh Rezwan

**1. What bugs did you find ? How did you solve these and why ?**

- **Bug 1:** Adding a user from the people tab was not displaying the user name. Fixed by updating the form name input and setting it as a property into the `values` object, to save the user name when adding a new user.
- **Bug 2:** The update button action in the user view page on form submit was set to onChange instead of onClick. Fixed to onClick to ensure the update operation works correctly.
- **Bug 3:** Clicking to view project details (in the project view page) after adding a project on the projects tab resulted in a crash error. This was because the fetched project details came in an array format. Fixed by accessing the object within the project array using `project[0]` and then accessing the properties of the object.
- **Bug 4:** The edit page of the projects tab was not correctly linked and resulted in `undefined`. Fixed by taking the first element of the project array to get the dynamic `_id` of the object found.
- **Bug 5:** In the project edit page, the loaded project was also in array form, causing issues and not showing the project data. Fixed by setting initial form values as project[0] and accessing key values in the same way.
- **Bug 6:** Users were unable to update their email address from the My account page. Fixed by allowing users to update their email using input name as email and updating user `values` using onChange.

**2. Which feature did you develop and why?**

- **Feature 1:** Now, the `availability` of the user can directly be changed from the user update form. This feature was implemented so that the project manager can conveniently update team members` availability status.
- **Feature 2:** Users can now update their `profile avatar` using a photo URL link from the My account page. This feature was added to enhance user customization options and improve the overall user experience.
- **Feature 3:** A small `pie chart visualization` for projects with the maximum budget known, against the budget consumed, was added. This feature provides users with a visual representation of project budget utilization, aiding in better budget management and decision-making.

**3. Do you have any feedback about the code/architecture of the project, and what difficulties did you encounter while doing it?**

- Overall, the codebase follows a structured architecture and adheres to best practices.
- However, there were some challenges encountered during development, particularly in handling data structures and managing state updates efficiently.
- Further optimization and refactoring may be beneficial to improve performance and maintainability in the long run.

---

Thank you for your time and consideration in checking my submission. I hope to hear from you soon.

Shaikh Rezwan
shaikhrezwan66@gmail.com
