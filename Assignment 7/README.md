# Assignment 7 - About Me Page

## 1. Aim
Build a short About Me page with semantic tags, an about section and a contact link.

## 2. Theoretical Background
- Semantic HTML5: Using meaningful tags like <header>, <nav>, <main>, <section>, and <footer> gives clear structure to content.
- In-page Navigation: Fragment identifiers (href="#about") jump to specific element IDs on the same page.
- mailto Links: Initiates email composition to the specified student address.

## 3. Tasks Breakdown
- Task 1: Semantic header with h1 name and navigation links (#about, #contact).
- Task 2: Main section with id="about", h2 heading "About me", and student bio paragraph.
- Task 3: Footer with id="contact" and a clickable mailto email link.

## 4. Code Listings

about-me.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>About Me | Daksh Thakur</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Daksh Thakur</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section id="about">
            <h2>About me</h2>
            <p>I am a second-year B.Tech Computer Science and Engineering student at Invertis University, Bareilly. I am currently learning front-end web development including semantic HTML5, CSS layout techniques, and modern version control with Git.</p>
        </section>
    </main>

    <footer id="contact">
        <p>Email: <a href="mailto:dakshthakur506@gmail.com">dakshthakur506@gmail.com</a></p>
    </footer>
</body>
</html>
```

style.css:
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

header {
    background-color: #f4f4f4;
    padding: 20px;
    border-bottom: 1px solid #ddd;
}

header h1 {
    margin: 0 0 10px 0;
}

header nav a {
    margin-right: 15px;
    text-decoration: none;
    color: #0066cc;
    font-weight: bold;
}

main {
    flex: 1;
    padding: 20px;
}

footer {
    background-color: #eee;
    padding: 15px 20px;
    border-top: 1px solid #ddd;
}
```

## 5. Output Verification
Semantic page rendering verified in the browser:

![Assignment 7 Output](images/screenshot.png)

## 6. Conclusion
A semantic HTML5 webpage with header, navigation, main section, and contact footer was created and tested.
