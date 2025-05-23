<!DOCTYPE html>
<html lang="en">
<head>
  <title>Quote of the Day</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f8ff;
      text-align: center;
      padding: 50px;
    }
    .quote-box {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      max-width: 500px;
      margin: auto;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }
    .quote-text {
      font-size: 20px;
      font-style: italic;
      margin-bottom: 15px;
    }
    .quote-author {
      font-weight: bold;
      margin-bottom: 20px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      border: none;
      background-color: #007BFF;
      color: white;
    }
  </style>
</head>
<body>
  <div class="quote-box">
    <p id="quote" class="quote-text">"The only way to do great work is to love what you do."</p>
    <p id="author" class="quote-author">- Steve Jobs</p>
    <button onclick="changeQuote()">Change Quote</button>
  </div>
  <script>
    var quotes = [
      {text: "The only way to do great work is to love what you do.", author: "Steve Jobs"},
      {text: "Believe you can and you're halfway there.", author: "Theodore Roosevelt"},
      {text: "You miss 100% of the shots you don’t take.", author: "Wayne Gretzky"},
      {text: "Success is not final, failure is not fatal: It is the courage to continue that counts.", author: "Winston Churchill"},
      {text: "Hard work beats talent when talent doesn’t work hard.", author: "Tim Notke"},
      {text: "Don’t watch the clock; do what it does. Keep going.", author: "Sam Levenson"}
    ];
    function changeQuote() {
      var randomIndex = Math.floor(Math.random() * quotes.length);
      var randomQuote = quotes[randomIndex];
      document.getElementById("quote").innerText = '"' + randomQuote.text + '"';
      document.getElementById("author").innerText = '- ' + randomQuote.author;
    }
  </script>
</body>
</html>
