# Responsive Webpage Exercise

## Objective

Create a simple, responsive webpage using basic HTML and SCSS, incorporating more elements, styles, and SCSS partials.

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

2. **SCSS Structure:**
    - Create a `styles.scss` file and several partials for organizing your SCSS code.
    - Create a folder named `partials` and add the following files:
        - `_variables.scss`
        - `_reset.scss`
        - `_header.scss`
        - `_main.scss`
        - `_footer.scss`
        - `_responsive.scss`

3. **SCSS Partials:**

    **`_variables.scss`**

    ```scss
    // Define variables
    $primary-color: #3498db;
    $secondary-color: #2ecc71;
    $font-stack: Helvetica, sans-serif;
    ```

    **`_reset.scss`**

    ```scss
    // Basic reset
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    ```

    **`_header.scss`**

    ```scss
    header {
        background: $primary-color;
        color: white;
        padding: 10px 0;
        text-align: center;

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
    }
    ```

    **`_main.scss`**

    ```scss
    main {
        margin: 20px 0;

        .intro {
            margin-bottom: 20px;

            img {
                max-width: 100%;
                height: auto;
                display: block;
                margin: 10px 0;
            }
        }

        .cards {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;

            .card {
                background: $secondary-color;
                color: white;
                padding: 20px;
                flex: 1;
                min-width: 200px;
                border-radius: 5px;
                text-align: center;
            }
        }
    }
    ```

    **`_footer.scss`**

    ```scss
    footer {
        background: #333;
        color: white;
        text-align: center;
        padding: 10px 0;
        margin-top: 20px;
    }
    ```

    **`_responsive.scss`**

    ```scss
    // Responsive Design
    @media (min-width: 600px) {
        body {
            padding: 40px;
        }

        header, footer {
            padding: 20px 0;
        }

        main {
            margin: 40px 0;

            .intro img {
                width: 80%;
                margin: 20px auto;
            }

            .cards {
                justify-content: space-around;

                .card {
                    flex: 0 0 30%;
                }
            }
        }
    }
    ```

4. **Main SCSS File:**

    **`styles.scss`**

    ```scss
    // Import partials
    @import 'partials/variables';
    @import 'partials/reset';
    @import 'partials/header';
    @import 'partials/main';
    @import 'partials/footer';
    @import 'partials/responsive';

    body {
        font-family: $font-stack;
        line-height: 1.6;
        padding: 20px;
    }
    ```

5. **Compile SCSS to CSS:**
    - Compile the SCSS file to CSS. This can be done using a tool like [Sass](https://sass-lang.com/install) or an online compiler.

6. **Link the CSS File:**
    - Ensure that the compiled `styles.css` file is linked correctly in the `index.html` file.

7. **Review and Test:**
    - Open the `index.html` file in a web browser.
    - Resize the browser window to see the responsive design in action.
    - Ensure all elements are styled and behave as expected.

8. **Commit and push your changes**

## Outcome

You should have a more comprehensive responsive webpage that looks good on both desktop and mobile devices, with a navigation menu, introductory section, and a card layout.
