# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Flexbox Page</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }

    /* Navigation */
    nav {
      background-color: #333;
      color: #fff;
      padding: 1rem;
    }

    nav ul {
      display: flex;
      justify-content: space-between;
      list-style: none;
      flex-wrap: wrap;
    }

    nav ul li {
      margin: 0.5rem;
    }

    nav a {
      color: white;
      text-decoration: none;
    }

    /* Layout */
    .container {
      display: flex;
      flex-direction: row;
      gap: 20px;
      padding: 20px;
    }

    .sidebar {
      flex: 1;
      background: #f4f4f4;
      padding: 10px;
    }

    .main {
      flex: 3;
      background: #eaeaea;
      padding: 10px;
    }

    /* Responsive Media Queries */
    @media (max-width: 768px) {
      .container {
        flex-direction: column;
      }

      nav ul {
        flex-direction: column;
        align-items: flex-start;
      }
    }

    @media (min-width: 769px) and (max-width: 1024px) {
      .container {
        flex-direction: row;
      }
    }

    @media (min-width: 1025px) {
      .container {
        flex-direction: row;
      }
    }
  </style>
</head>
<body>

  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Projects</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <div class="container">
    <div class="sidebar">
      <h2>Sidebar</h2>
      <p>This is the sidebar content.</p>
    </div>
    <div class="main">
      <h2>Main Content</h2>
      <p>This is where your main content goes.</p>
    </div>
  </div>

</body>
</html>

