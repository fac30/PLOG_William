## Guidance
Answer the following questions considering the learning outcomes for
- [Week 04](https://learn.foundersandcoders.com/course/syllabus/developer/week04-project03-frontend/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- Learn how to integrate TypeScript with a React (S1, S11, S16)

Used the command to start the typescript react frontend and configure its settings.
 ```
  npm install --save typescript @types/node @types/react @types/react-dom @types/jest
  ```
 - Understand the concepts of components, props, and state in React
```
// used state variables to control selected values in a dropdown menu
const Questions: React.FC = () => {
  const [questions, setQuestions] = useState<Question[]>([]);
  const [currentQuestionIndex, setCurrentQuestionIndex] = useState(0);
// code...
useEffect(() => {
    const storedQuizData = localStorage.getItem('quizData');
    if (storedQuizData) {
      setQuestions(JSON.parse(storedQuizData).questions);
// more code...
```
- Implement routing in a single-page application using React Router
Inside App.tsx:
```
// imports
 <Router>
      <Routes>
        <Route path="/" element={<Home />} />
// more routes...
```
- Manage global state and side-effects in React applications

Used useEffect to control redirects if certain state variables or conditions are met:
```
 useEffect(() => {
    const storedQuizData = localStorage.getItem('quizData');
    if (storedQuizData) {
      setQuestions(JSON.parse(storedQuizData).questions);
    } else {
      navigate('/settings');
    }
  }, [navigate]);
```
- Create reusable UI components and manage their lifecycle
Example button component:
```
const Button: React.FC<ButtonProps> = ({ label, onClick, classes, disabled = false, status = 'default' }) => {
// code...
<button className={buttonClasses} onClick={onClick} disabled={disabled}>
      {label}
    </button>
```
- Handle asynchronous operations and manage data fetching in React

Inside question fetcher in Settings.tsx:
```
try {
    const response = await fetch(
      `http://localhost:5000/api/quiz?difficulty=${selectedDifficulty}&type=${quizType}&numberOfQuestions=${parseInt(selectedNumberOfQuestions, 10)}`
    );
// code...
//...
// catch block
```

- Set environment variables and understand their use case

A ```.env.template``` file is created in the backend to show how environment variables should be labelled to use.

 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- Draw a diagram representing the flow of our application

Need to write documentation and perhaps create a diagram to describe the request and response loop of our project.

## Feedback (For CF's)
> [**Course Facilitator name**]

Alexander

> [*What went well*]

Great explanations and great code snippets. Quite concise and right to the point

> [*Even better if*]


