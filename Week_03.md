## Guidance
Answer the following questions considering the learning outcomes for
- [Week 03](https://learn.foundersandcoders.com/course/syllabus/developer/week03-project03-server/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- Develop a server using Express and TypeScript for backend applications
```
// app.ts
// imports...
const PORT = process.env.PORT || 5000;
const app = express();
// code...
```
- Identify the server’s role within a full stack application
```
// Handling requests:
app.use('/api/quiz', quizRoutes);
// direct to quiz route file in /src/routes/quizRoutes.ts

// Process the request
// inside the route pass the controller to process the request

router.get('/', getQuiz);

// inside the controller in /src/controllers/quizController
// process request and respond with a json object back to the client

export const getQuiz = async (req: Request, res: Response) => {
// code
res.json(quiz)
// error handling
```

- Understand the benefits of using TypeScript over JavaScript, such as improved code quality, enhanced developer productivity, and better tooling support 
```
// used type saftey to check inputs inside async function
export const getCountries = async (req: Request, res: Response) => {
// code
}
```
### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- Learn the basic syntax and features of TypeScript
(need to write more typescript to better understand its syntax and benefits)
- Grasp the concept and purpose of RESTful APIs / Construct and implement RESTful APIs effectively
- (will need to add more data and create more routes/controllers to have a better grasp on the idea of RESTful API and the design constraints of the interface to share and modify data from the database.
```
// currently only connected to the database and provided a test route '/countries' to fetch some data
router.get('/', getCountries);
// /src/controllers/getCountries.ts
export const getCountries = async (req: Request, res: Response) => {
  try {
    const [rows] = await db.query('SELECT * FROM countries');
    res.json(rows);
```
## Feedback (For CF's)
> [**Course Facilitator name**]

Alexander

> [*What went well*]

Perfect code snippets, minimal and to the point.

> [*Even better if*]

There is no need to include generic learnings, like "Learn the basic syntax and features of TypeScript (need to write more typescript to better understand its syntax and benefits)" since this is never going to be checked in the future. Consider your PLog more like a cheatsheet for yourself, or even a place were you can redirect someone who is struggling with same things as you
