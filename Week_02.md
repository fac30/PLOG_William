## Guidance
Answer the following questions considering the learning outcomes for
- [Week 02](https://learn.foundersandcoders.com/course/syllabus/developer/week02-project02-chatbot/learning-outcomes/)

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- Write code that executes asynchronously:
```
async execute(interaction) {
    // Initialize a 3x3 board for the Tic Tac Toe game, represented by emojis.
    /*
    code...
    */
await interaction.reply({
      content: "Tic Tac Toe started! Click on a button to play!",
      components: createGrid(),
    });
```
- Use callbacks to access values that aren’t available synchronously:
```
 // Handle each button click event (move)
    collector.on("collect", async (i) => {
  /// code...
  await interaction.editReply({
        content: `Tic Tac Toe ongoing! ${currentPlayer}'s turn`,
        components: createGrid(),
      });
    });
```
- Use promises to access values that aren’t available synchronously:
- Use the fetch method to make HTTP requests and receive responses:
- Configure the options argument of the fetch method to make GET and POST requests
```
 async execute(interaction) {
        try {
            // Send a message to the user that the image is loading
            await interaction.reply('loading image');
            
            // Fetch memes from the Imgflip API
            const response = await fetch('https://api.imgflip.com/get_memes', {
                method: 'GET', // Correct the 'Method' to lowercase 'method'
            });
```
- Set up a Node.js environment for web development
```
// Creates new client
const client = new Discord.Client({
  intents: [
    Discord.GatewayIntentBits.Guilds,
    Discord.GatewayIntentBits.MessageContent,
    Discord.GatewayIntentBits.GuildMessages,
  ],
});

const discordToken = process.env.DISCORD_TOKEN;
```
- Use environment variables for managing secrets and sensitive keys in Node.js:

A .env.template file is setup to show example of how to label keys.

- Use npm to manage project dependencies and scripts in a Node.js environment.

Project dependecencies and scripts are written and listed in the package.json.


 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- Write tests to mimic the behaviour of a user performing different actions.

Would like to explore integration testing a bit more to combine all unit tests together.
Write tests for asynchronous functions.

## Feedback (For CF's)
> [**Course Facilitator name**]  
> [*What went well*]  
> [*Even better if*]
