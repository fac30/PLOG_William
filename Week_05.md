## Guidance
Answer the following questions considering the learning outcomes for
- [Week 05](https://learn.foundersandcoders.com/course/syllabus/developer/week05-project03-test-deploy/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- Learn how to write and run unit tests for backend functionality using the Node testing suite and Postman.
```
describe('GET /countries', () => {
  let server: http.Server;
// code ...
it('should return a list of countries.', async () => {
    const mockData = [
      {
        id: 1,
        country: 'France',
        capital: 'Paris',
        capital_difficulty: 'easy',
        country_code: 'FR',
      },
// more code...
```
- Gain experience in using the Cypress testing library with React.
```
// including configuration and using the cypress app:
describe("This is a sample test.", () => {
  it("Visits localhost/5173", () => {
    cy.visit("http://localhost:5173/");
  });
});
```

- Gain experience in deploying a full-stack web application to a cloud platform
Deployed a database on RDS and backend server onto an EC2 instance. Automated deployment on Amplify.

- Understand the differences between development, staging, and production environments.
Created a staging branch to push changes which would then be merged into main branch for deployment.

- Configure the necessary environment variables and settings for deployment
Used IS_PRODUCTION environment variable to control the behaviour of route controllers.

- Gain experience in using a continuous integration and deployment (CI/CD) pipeline
Created workflows in .github/workflows to automate pull request processes.

 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- Would like to revisit creating routes and controlling data sent to the frontend.
- Testing routes and functionality of the backend.

## Feedback (For CF's)
> [**Course Facilitator name**]

Alexander

> [*What went well*]

Basic understanding of testing setup with both unit tests and Cypress. Good grasp of environment separation and deployment workflow concepts.

> [*Even better if*]

Add more complex test examples, your current ones only show basic configuration. Since you mentioned struggling with routes and backend testing, show specific examples of what routes gave you trouble.
