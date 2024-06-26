# Technical test

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

- Overall, the codebase follows quite a complex architecture but adheres to best practices.
- However, I think that there were some challenges faced during development, particularly in handling data structures and managing state updates efficiently.
- Further optimization and refactoring may help to improve performance and maintainability in the long run.
- One major bug was related to the login functionality, where a signed up user is unable to login using their Username and Password. Despite recognizing the problem, I encountered difficulty in resolving it due to the complexity and abstract nature of the signin and signup pages' code. While I was unable to address this issue directly, I remain committed and want to collaborate to find a solution.

---

Thank you for your time and consideration in checking my submission. I hope to hear from you soon.

Shaikh Rezwan
[Submission Repo](https://github.com/Rezwan66/shaikh-selego-technical-test-2)
shaikhrezwan66@gmail.com
