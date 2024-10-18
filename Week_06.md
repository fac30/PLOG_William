## Guidance
Answer the following questions considering the learning outcomes for
- [Week 06](https://learn.foundersandcoders.com/course/syllabus/developer/week06-project04-databases/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- Learn how to design and structure a database schema for the application
- ![image](https://github.com/user-attachments/assets/711a64aa-c2f2-4b0e-bb03-10b1e7d8dd70)

- Implement CRUD (Create, Read, Update, Delete) operations for products and orders
```
// from controllers:
const getAllTutorsController = (req: Request, res: Response) => {
  const tutors = getAllTutors();
  if (tutors) {
    res.json(tutors);
// ... code

//from models:
const tutors = zubiDB.prepare("SELECT * FROM tutors");

const allRows = tutors.all();

const getTutorById = (index: number) => {
  return allRows[index - 1];
};
```
-Acquire skills in using SQLite to manage and query relational data efficiently
Created a database config file in the project database folder and a seeding file which would create and seed the database with data after running an npm script.
Querying the database is placed in the models folder that is connected to controllers which are called based on the route from the request.

- Be comfortable with SQL syntax and how to use SELECT and INSERT queries
Used sql syntax to create and insert data using a schema file.


 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- Testing the crud operations similar to how it was done in the workshop to gain a better understanding of unit testing and eventually build towards integration testing for server routes.

## Feedback (For CF's)
> [**Course Facilitator name**]  
> [*What went well*]  
> [*Even better if*]
