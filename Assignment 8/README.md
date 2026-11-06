# Assignment 8 - Sign-Up Forms and Choices

## 1. Aim
Make a labelled form with text, email and password fields, choices and a submit button.

## 2. Theoretical Background
- The form Element: Handles user input submission using method and action attributes.
- Label Association: Linking <label for="id"> with <input id="id"> improves usability and accessibility.
- Input Types: text, email, password, radio buttons, and select dropdowns.
- Validation: The required attribute enforces mandatory fields, and placeholder gives transient guidance.

## 3. Tasks Breakdown
- Task 1 (signup.html): Form with method="post" action="thanks.html" and linked labels for Full Name, Email, Password.
- Task 2 (choices.html): Gender radio buttons (Female, Male) and course select dropdown (BCA, B.Tech).
- Task 3 (signup-required.html): Required Full Name with placeholder, required Email, and Submit button.

## 4. Code Listings

signup.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Sign Up</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>Student Registration</h2>
    <form method="post" action="thanks.html">
        <div class="form-group">
            <label for="fullname">Full Name:</label>
            <input type="text" id="fullname" name="fullname">
        </div>

        <div class="form-group">
            <label for="useremail">Email Address:</label>
            <input type="email" id="useremail" name="useremail">
        </div>

        <div class="form-group">
            <label for="userpassword">Password:</label>
            <input type="password" id="userpassword" name="userpassword">
        </div>

        <button type="submit">Sign Up</button>
    </form>
</body>
</html>
```

choices.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Choices Form</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>Course and Gender Selection</h2>
    <form>
        <p><strong>Select Gender:</strong></p>
        <label><input type="radio" name="gender" value="female"> Female</label>
        <label><input type="radio" name="gender" value="male"> Male</label>

        <p><strong>Select Course:</strong></p>
        <label for="course">Course:</label>
        <select id="course" name="course">
            <option value="BCA">BCA</option>
            <option value="B.Tech">B.Tech</option>
        </select>
    </form>
</body>
</html>
```

signup-required.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Required Sign Up</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>Mandatory Student Sign Up</h2>
    <form>
        <div class="form-group">
            <label for="req-name">Full Name:</label>
            <input type="text" id="req-name" name="fullname" placeholder="Enter full legal name" required>
        </div>

        <div class="form-group">
            <label for="req-email">Email Address:</label>
            <input type="email" id="req-email" name="email" required>
        </div>

        <button type="submit">Submit</button>
    </form>
</body>
</html>
```

style.css:
```css
body {
    font-family: Arial, sans-serif;
    margin: 20px;
    line-height: 1.6;
    color: #333;
}

h2 {
    color: #222;
}

form {
    max-width: 400px;
    padding: 15px;
    border: 1px solid #ccc;
    background-color: #fafafa;
}

.form-group {
    margin-bottom: 12px;
}

label {
    display: block;
    margin-bottom: 4px;
    font-weight: bold;
}

input[type="text"],
input[type="email"],
input[type="password"],
select {
    width: 100%;
    padding: 8px;
    box-sizing: border-box;
    border: 1px solid #ccc;
}

button {
    padding: 8px 16px;
    background-color: #0066cc;
    color: white;
    border: none;
    cursor: pointer;
    margin-top: 10px;
}
```

## 5. Output Verification
Form elements rendered and validated in the browser:

![Assignment 8 Output](images/screenshot.png)

## 6. Conclusion
Labelled form inputs, radio buttons, dropdown choices, and HTML5 required attributes were successfully implemented.
