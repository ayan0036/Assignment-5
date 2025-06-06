# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flexbox Layout</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    header {
      background-color: #4CAF50;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #333;
      color: white;
      display: flex;
      justify-content: space-around;
      padding: 10px;
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 8px 12px;
    }

    nav a:hover {
      background-color: #575757;
      border-radius: 4px;
    }

    .main {
      display: flex;
      flex: 1;
      padding: 20px;
      gap: 20px;
    }

    .content, .sidebar {
      padding: 20px;
      background-color: #f4f4f4;
      border-radius: 5px;
    }

    .content {
      flex: 2;
    }

    .sidebar {
      flex: 1;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 15px;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      .main {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>My Flexbox Website</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Services</a>
    <a href="#">Contact</a>
  </nav>

  <div class="main">
    <div class="content">
      <h2>Main Content</h2>
      <p>This is the main area of the page. You can put articles, blog posts, or any important content here.</p>
    </div>

    <div class="sidebar">
      <h2>Sidebar</h2>
      <p>This section can contain links, additional info, or advertisements.</p>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 My Website. All rights reserved.</p>
  </footer>

</body>
</html>
