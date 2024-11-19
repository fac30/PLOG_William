## Guidance
Answer the following questions considering the learning outcomes for
- [Week 07](https://learn.foundersandcoders.com/course/syllabus/developer/week07-project04-authentication/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.

1.  Learn how to handle user registration, login, and logout functionality securely (K8, S17, B5)
    - Created authentication routes in the routes folder to handle login , logout and status checks for the client.
    - Used passport.js package with local strategy to design and build an authentication method to handle login. Strategy is stored in the auth folder inside src.
    - Used bcrypt to compare user input password and the hashed password that is stored in the database.

2. Understand the principles of authentication and authorisation in web applications
   - Used video guide and documentation to first understand how cookies worked and creating sessions with express-session.js. Created a test route called cookies to understand the concepts in the guide and documentation as well as added comments to share knowledge with the team.

3. Develop strategies to mitigate security threats such as Cross-site Request Forgery (CSRF) attacks
   - Following the workshop, documentation and video guides, made changes to the cookie settings in the server object like:
```
cookie: {
      secure: false, // Set to `true` if using HTTPS
      maxAge: 24 * 60 * 60 * 1000, // 1-day cookie expiry
      sameSite: "strict",
      httpOnly: true,
    },
```
to control access and usage of the cookies from the client.

4. Implement navigation between different pages using React Router
   - In the frontend repo, we created routes for different pages of our website:
     ``` jsx
     // code...
     <BrowserRouter>
        <Routes>
          <Route path="/" element={<Home />} />
          <Route path="/about" element={<About />} />
     // mode code...

 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
1.  Learn how to handle user registration, login, and logout functionality securely (K8, S17, B5)
    - Although the login and logout functionality is implemented with the frontend, the routes still require middleware to thoroghly handle errors from the passport strategy and checking for logged in status for certain routes such as for booking a study session.
    - Understand the data the frontend needs to transform the ui, such as the username or account name that can be used to display on the navbar.

## Feedback (For CF's)
> [**Course Facilitator name**]

Alexander

> [*What went well*]

Good implementation of secure authentication with proper cookie configuration. Clear understanding of Passport.js local strategy and bcrypt for password handling.

> [*Even better if*]

Show the actual Passport.js strategy implementation you mentioned. Since you noted struggles with middleware error handling, include examples of your current error handling code that needs improvement.
