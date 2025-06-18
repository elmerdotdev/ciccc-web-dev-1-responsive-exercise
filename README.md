# Web 1 - Responsive Webpage Exercise

**Goal:** Create a simple, responsive webpage using basic HTML and CSS. You’ll build a well-structured layout and add your own media queries to make it responsive.

## Instructions ✅

1. **HTML Structure:**
    - Create an `index.html` file and copy the following code into it:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Responsive Webpage</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <header>
            <h1>My Responsive Webpage</h1>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </header>
        <main>
            <section class="intro">
                <h2>Welcome to My Website</h2>
                <p>This is a simple responsive webpage. Resize the browser window to see the effect!</p>
                <img src="https://placehold.co/800x400.png" alt="Sample Image">
            </section>
            <section class="cards">
                <div class="card">
                    <h3>Card 1</h3>
                    <p>This is the first card.</p>
                </div>
                <div class="card">
                    <h3>Card 2</h3>
                    <p>This is the second card.</p>
                </div>
                <div class="card">
                    <h3>Card 3</h3>
                    <p>This is the third card.</p>
                </div>
            </section>
        </main>
        <footer>
            <p>© 2024 Your Name</p>
        </footer>
    </body>
    </html>
    ```

2. **CSS Styles:**
    - Create a `styles.css` file and copy the following CSS code:

    ```css
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        font-family: Helvetica, sans-serif;
        line-height: 1.6;
        padding: 20px;
    }

    header {
        background: #3498db;
        color: white;
        padding: 10px 0;
        text-align: center;
    }

    nav ul {
        list-style: none;
        padding: 0;
    }

    nav li {
        display: inline;
        margin: 0 10px;
    }

    nav a {
        color: white;
        text-decoration: none;
    }

    main {
        margin: 20px 0;
    }

    .intro {
        margin-bottom: 20px;
    }

    .intro img {
        max-width: 100%;
        height: auto;
        display: block;
        margin: 10px 0;
    }

    .cards {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
    }

    .card {
        background: #2ecc71;
        color: white;
        padding: 20px;
        flex: 1;
        min-width: 200px;
        border-radius: 5px;
        text-align: center;
    }

    footer {
        background: #333;
        color: white;
        text-align: center;
        padding: 10px 0;
        margin-top: 20px;
    }
    ```

3. **Add Responsive Behavior:**
    - Now it’s your turn to make the page responsive. Add a media query at the **bottom of your CSS file** that applies when the viewport width is **600px or wider**.
    - Inside the media query, apply the following changes:
        - Increase `body` padding to `40px`
        - Increase padding on the `header` and `footer` to `20px 0`
        - Set `.intro img` width to `80%` and center it using `margin: 20px auto`
        - In the `.cards` section:
            - Use `justify-content: space-around`
            - Make each `.card` have `flex: 0 0 30%`

    - Example (to be written by you):

    ```css
    /* Add this at the bottom of styles.css */
    @media (min-width: 600px) {
        /* Your changes go here */
    }
    ```

4. **Review and Test:**
    - Open your `index.html` file in a browser.
    - Resize the window and verify your responsive changes work correctly.

5. **Commit and Push Your Changes**
