# Assignment 12 - Box Model, Cards and Scrolling

## 1. Aim
Compare content-box and border-box, build a styled card, and add a scrolling box.

## 2. Theoretical Background
- **CSS Box Model**: Composed of content, padding, border, and margin.
  - `content-box` (default): Width and height apply to content only; padding and border add to the element's rendered size.
  - `border-box`: Width and height include content, padding, and border.
- **Card UI**: Utilizes border, padding, border-radius, and box-shadow to create a card component.
- **Overflow Control**: `overflow: auto` adds scrollbars only when content exceeds the container boundaries.

## 3. Tasks Breakdown
- **Task 1 (`box-model.html`)**: Two boxes with identical width, height, padding, and border, contrasting `box-sizing: content-box` vs `border-box`.
- **Task 2 (`card.html`)**: Styled `.card` element with a border, 16px padding, rounded corners (`border-radius`), a light shadow (`box-shadow`), a heading, and two sentences.
- **Task 3 (`scroll.html`)**: Fixed 200px by 200px box with `overflow: auto` and enough text to produce a vertical scrollbar.

## 4. Code Listings

### box-model.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Box Sizing Comparison</title>
    <style>
        .box {
            width: 250px;
            height: 100px;
            padding: 20px;
            border: 5px solid #333333;
            margin-bottom: 25px;
        }
        .content-box {
            box-sizing: content-box;
            background-color: #e0f2fe;
        }
        .border-box {
            box-sizing: border-box;
            background-color: #dcfce7;
        }
    </style>
</head>
<body>
    <div class="box content-box">
        <strong>Box 1 (content-box):</strong> Total width = 250px + 40px padding + 10px border = 300px.
    </div>

    <div class="box border-box">
        <strong>Box 2 (border-box):</strong> Total width stays exactly 250px.
    </div>
</body>
</html>
```

### card.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Card Component</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8fafc;
            padding: 40px;
        }
        .card {
            border: 1px solid #cbd5e1;
            padding: 16px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            background-color: #ffffff;
            max-width: 320px;
        }
        .card h2 {
            margin-top: 0;
            color: #1e293b;
        }
        .card p {
            color: #475569;
            line-height: 1.5;
            margin-bottom: 0;
        }
    </style>
</head>
<body>
    <div class="card">
        <h2>Web Development Fundamentals</h2>
        <p>This introductory module provides essential skills for creating structured and styled websites. Students learn to implement responsive layouts and clean modern components.</p>
    </div>
</body>
</html>
```

### scroll.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Overflow and Scrolling</title>
    <style>
        .scroll-container {
            width: 200px;
            height: 200px;
            overflow: auto;
            border: 2px solid #334155;
            padding: 12px;
            background-color: #f8fafc;
            box-sizing: border-box;
        }
    </style>
</head>
<body>
    <div class="scroll-container">
        <h3>Scrollable Content</h3>
        <p>Paragraph 1: CSS overflow property controls what happens when content exceeds the dimensions of an element box.</p>
        <p>Paragraph 2: When set to auto, scrollbars automatically appear only when the content extends beyond the box boundary.</p>
        <p>Paragraph 3: This ensures responsive readability without distorting page layouts.</p>
        <p>Paragraph 4: Additional lines ensure the vertical scrollbar is active and visible.</p>
    </div>
</body>
</html>
```

## 5. Output Verification
Card UI component output in browser (`card.html`):

![Assignment 12 Output](images/screenshot.png)

## 6. Conclusion
Box-sizing properties were analyzed, a card with shadow and padding was built, and overflow auto scrollbars were verified.
