# Web 1 - Responsive Webpage Exercise

## Objective

Create a simple, responsive webpage using basic HTML and CSS, incorporating multiple elements and styles.

## Instructions

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
                <img src="https://via.placeholder.com/800x400" alt="Sample Image">
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
    - Create a `styles.css` file and copy the following code into it:

    ```css
    /* Reset */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    /* Variables (using direct values in CSS) */
    body {
        font-family: Helvetica, sans-serif;
        line-height: 1.6;
        padding: 20px;
    }

    /* Header */
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

    /* Main Content */
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

    /* Footer */
    footer {
        background: #333;
        color: white;
        text-align: center;
        padding: 10px 0;
        margin-top: 20px;
    }

    /* Responsive Design */
    @media (min-width: 600px) {
        body {
            padding: 40px;
        }

        header,
        footer {
            padding: 20px 0;
        }

        main {
            margin: 40px 0;
        }

        .intro img {
            width: 80%;
            margin: 20px auto;
        }

        .cards {
            justify-content: space-around;
        }

        .card {
            flex: 0 0 30%;
        }
    }
    ```

3. **Review and Test:**
    - Open `index.html` in your browser.
    - Resize the window to test the responsiveness.
    - Ensure all styles are applied correctly and elements adapt to different screen sizes.

4. **Commit and Push Your Changes:**
    - Save your work and push your files to your version control system (e.g., GitHub).

## Outcome

You should have a well-structured, responsive webpage that looks great on both desktop and mobile devices. It should include a header, navigation, an intro section, a responsive card layout, and a footer.
