CSS

/* General styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

/* Navbar styles */
#navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 200px;
    height: 100%;
    background-color: #333;
    color: white;
    padding: 20px;
}

#navbar header {
    font-size: 1.5em;
    margin-bottom: 20px;
}

.nav-link {
    display: block;
    color: white;
    text-decoration: none;
    margin: 10px 0;
}

.nav-link:hover {
    text-decoration: underline;
}

/* Main content */
#main-doc {
    margin-left: 220px;
    padding: 20px;
    max-width: 800px;
}

.main-section {
    margin-bottom: 40px;
}

header {
    font-size: 2em;
    margin-bottom: 10px;
}

code {
    background-color: #f4f4f4;
    padding: 5px;
    display: block;
    margin: 10px 0;
}

/* Responsive design */
@media (max-width: 600px) {
    #navbar {
        display: none;
    }
    
    #main-doc {
        margin-left: 0;
    }
}

HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Technical Documentation</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- Navbar -->
    <nav id="navbar">
        <header>Documentation</header>
        <a class="nav-link" href="#Introduction">Introduction</a>
        <a class="nav-link" href="#HTML_Basics">HTML Basics</a>
        <a class="nav-link" href="#CSS_Overview">CSS Overview</a>
        <a class="nav-link" href="#JavaScript_Fundamentals">JavaScript Fundamentals</a>
        <a class="nav-link" href="#Responsive_Design">Responsive Design</a>
    </nav>

    <!-- Main Documentation Content -->
    <main id="main-doc">

        <!-- Section 1 -->
        <section class="main-section" id="Introduction">
            <header>Introduction</header>
            <p>This documentation provides an overview of essential web development concepts.</p>
            <p>We will cover HTML, CSS, JavaScript, and responsive design principles.</p>
        </section>

        <!-- Section 2 -->
        <section class="main-section" id="HTML_Basics">
            <header>HTML Basics</header>
            <p>HTML (Hypertext Markup Language) is the structure of web pages.</p>
            <p>It defines elements like paragraphs, headings, lists, and images.</p>
            <code>&lt;p&gt;This is a paragraph.&lt;/p&gt;</code>
            <ul>
                <li>HTML tags are surrounded by angle brackets.</li>
                <li>HTML documents must have a <code>&lt;!DOCTYPE html&gt;</code> declaration.</li>
                <li>HTML elements can have attributes like class and id.</li>
            </ul>
        </section>

        <!-- Section 3 -->
        <section class="main-section" id="CSS_Overview">
            <header>CSS Overview</header>
            <p>CSS (Cascading Style Sheets) controls the visual design of web pages.</p>
            <p>It manages colors, fonts, and layouts to make websites attractive.</p>
            <code>body { background-color: lightblue; }</code>
            <ul>
                <li>CSS uses selectors to apply styles to HTML elements.</li>
                <li>It consists of properties and values.</li>
                <li>It allows for responsive design using media queries.</li>
            </ul>
        </section>

        <!-- Section 4 -->
        <section class="main-section" id="JavaScript_Fundamentals">
            <header>JavaScript Fundamentals</header>
            <p>JavaScript adds interactivity and dynamic behavior to web pages.</p>
            <p>It manipulates HTML and CSS and handles user interactions.</p>
            <code>document.querySelector('h1').style.color = 'red';</code>
            <ul>
                <li>JavaScript is executed on the client side.</li>
                <li>It handles events like clicks and form submissions.</li>
                <li>JavaScript can fetch data from APIs and update the page dynamically.</li>
            </ul>
        </section>

        <!-- Section 5 -->
        <section class="main-section" id="Responsive_Design">
            <header>Responsive Design</header>
            <p>Responsive design ensures that web pages look good on all screen sizes.</p>
            <p>It uses flexible layouts, media queries, and fluid grids.</p>
            <code>@media (max-width: 600px) { #navbar { display: none; } }</code>
            <ul>
                <li>Responsive design adapts content to different devices.</li>
                <li>Media queries allow for custom styles based on screen size.</li>
                <li>Flexible images and layouts adjust to fit different resolutions.</li>
            </ul>
        </section>

    </main>

</body>
</html>
