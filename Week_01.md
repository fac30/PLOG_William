## Guidance

Answer the following questions considering the learning outcomes for

- [Week 01](https://learn.foundersandcoders.com/course/syllabus/developer/week01-project01-basics/learning-outcomes/)
  
Make sure to record evidence of your processes. You can use code snippets, screenshots or any other material to support your answers.

Do not fill in the feedback section. The Founders and Coders team will update this with feedback on your progress.

Assessment
1. Show evidence of some of the learning outcomes you have achieved this week.
    - Structure a site using semantic HTML to aid accessibility
    - ```
      <article class="about-card" tabindex="0" aria-label="team-member-2">
            <img
              src="./assets/profile-images/Portrait of Derek Hernandez.jpg"
              alt="Derek's portrait"
            />
            <h3><strong>Derek Hernandez</strong></h3>
            <p>Job Title: Software Developer</p>
            <p>Favorite Genre: Science Fiction</p>
            <p>
              I’m a huge sci-fi fan. Films like Blade Runner and The Matrix
              really inspire me, especially when it comes to coding. I love
              diving deep into movie analysis and drawing parallels between film
              tech and real tech. In my spare time, I’ve been working on my own
              short sci-fi film, experimenting with CGI and futuristic themes
            </p>
          </article>
      ```
    - Use CSS Flexbox to style children in a single-direction layout (ie a row or a column)
    - ```
      .about-container {
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        justify-content: space-evenly;
      }
      ```
    - Use the appropriate input types in HTML forms for gathering different types of information
    - Ensure that forms are accessible and include appropriate labeling for screen readers
   - ```
      <div class="contact-container" role="form">
            <form
              action="#"
              method="post"
              onsubmit=""
              class="contact-form"
              aria-label="contact-heading"
            >
              <label class="form-label" for="contact-first-name">
                First Name
              </label>
              <input
                type="text"
                name="contact-first-name"
                id="contact-first-name"
                required
                aria-required="true"
                placeholder="Name..."
              />
              <label class="form-label" for="contact-last-name">
                Last Name
              </label>
              <input
                type="text"
                name="contact-last-name"
                id="contact-last-name"
                required
                aria-required="true"
                placeholder="Last Name..."
              />
              <label class="form-label" for="contact-email"> Email </label>
              <input
                type="email"
                name="contact-email"
                id="contact-email"
                required
                aria-required="true"
                placeholder="Email..."
              />
              <label class="form-label" for="contact-message">
                Work with us!
              </label>
              <textarea
                type="textarea"
                name="contact-message"
                id="contact-message"
                rows="10"
                cols="50"
                required
                aria-required="true"
                placeholder="Hello World!"
              ></textarea>
              <button type="submit" id="contact-submit" aria-label="submit form">
                submit
              </button>
            </form>
          </div>
     ```

3. Show an example of some of the learning outcomes you have struggled with and/or would like to re-visit.
  - Use CSS variables to apply repeated colours to HTML elements
  - ```
    body {
    line-height: 1;
    }
    ol,
    ul {
      list-style: none;
    }
    blockquote,
    q {
      quotes: none;
    }
    blockquote:before,
    blockquote:after,
    q:before,
    q:after {
      content: "";
      content: none;
    }
    table {
      border-collapse: collapse;
      border-spacing: 0;
    }
    
    html {
      overflow-x: hidden;
      position: relative;
      scroll-behavior: smooth;
    }
    
    body {
      overflow-x: hidden;
      position: relative;
      background-color: black;
      font-family: "space grotesk", sans-serif;
      color: white;
      font-size: 16px;
    }
    ```

Feedback (For CF's)
[Course Facilitator name]
[What went well]
[Even better if]
