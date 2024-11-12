## Guidance
Answer the following questions considering the learning outcomes for Week 09

Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

## Assessment
 ### 1. Show evidence of some of the learning outcomes you have achieved this week.
- created a simple web page using tailwind templates and refactored into views.
  ``` php
  <!DOCTYPE html>
  <html> 
      <?php require("./views/partials/head.php") ?>
      <body>
          <div class="min-h-full">
              <?php require('./views/partials/nav.php'); ?>
              <?php require('./views/partials/banner.php'); ?>
              <main>
                  <div class="mx-auto max-w-7xl px-4 py-6 sm:px-6 lg:px-8">
                  <p>Welcome to <?=$heading ?> page</p>
                  </div>
              </main>
          </div>
  
      </body>
  </html>
  ```
- from views, reused html is refactored into partials (smaller components).
  ``` php
  <head>
    <meta charset="UTF-8">
    <title>Section 2</title>
    <script src="https://cdn.tailwindcss.com"></script>
  </head>
  ```
- created a router to control what page is served by checking the request URI.
  ``` php
  $routes = [
    '/' => 'controllers/home.php',
    '/index.php' => 'controllers/home.php',
    '/about' => 'controllers/about.php',
    '/notes' => 'controllers/notes.php',
    '/note' => 'controllers/note.php',
  ];
  ```
- from routers, specific controllers is served respective of URI.
  ``` php
  <?php
  $heading = "Home";
  require "./views/index.view.php";  
  ?>
  ```
- created a simple mysql database with XAMPP, to test connecting a web server to the database using PHP.
  ``` php
  //Database.php
  ```
- displayed data from the database by making fetch calls to the database
  ```
  <?php
  $heading = 'Notes';
  $config = require 'config.php';
  
  $database = new Database($config['database']);
  
  $notes = $database->query('select * from notes where user_id = 3')->fetchAll();
  
  
  require "./views/notes.view.php";
  ?>
  ```

 ### 2. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
- error handling
- authentication
- cookies
- testing

## Feedback (For CF's)
> [**Course Facilitator name**]

Alexander

> [*What went well*]  

This is a great progress for your first week with PHP. It is also great how you always take into consideration testing, even if it is only as something you want to revisit in the near future.
