<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Webpage with HTML, CSS, and JavaScript</title>
  <style>
    /* CSS Styles */
    /* Reset some basic styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    /* Body styles */
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
      color: #333;
      text-align: center;
      padding: 50px;
      transition: background-color 0.5s ease;
    }
    /* Header styling */
    header {
      background-color: #2196F3;
      padding: 15px;
      color: white;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    h1 {
      font-size: 3em;
    }
    /* Button styling */
    .cta-button {
      padding: 20px 30px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 10px;
      font-size: 1.5em;
      cursor: pointer;
      transition: background-color 0.5s ease;
    }
    .cta-button:hover {
      background-color: #3e8e41;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to My Interactive Webpage</h1>
  </header>
  <main>
    <p>This is a simple webpage with HTML, CSS, and JavaScript.</p>
    <button class="cta-button" onclick="changeBackgroundColor()">Change Background Color</button>
    <button class="cta-button" onclick="changeTextColor()">Change Text Color</button>
  </main>
  <script>
    // JavaScript function to change the background color
    function changeBackgroundColor() {
      // Array of colors to choose from
      const colors = ["#f4f4f4", "#FFDDC1", "#D4E157", "#81C784", "#FFEB3B", "#FF5722"];
      // Randomly pick a color from the array
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      // Set the background color to the randomly selected color
      document.body.style.backgroundColor = randomColor;
    }
    
    // JavaScript function to change the text color
    function changeTextColor() {
      // Array of colors to choose from
      const colors = ["#333", "#666", "#999", "#CCC", "#FFF"];
      // Randomly pick a color from the array
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      // Set the text color to the randomly selected color
      document.body.style.color = randomColor;
    }
  </script>
</body>
</html>
