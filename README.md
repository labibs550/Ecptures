!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>IGCSE Economics Study Hub</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f0f4f8;
      color: #333;
      margin: 0;
      padding: 0 20px;
    }
    header {
      background: #4a90e2;
      color: white;
      padding: 20px 0;
      text-align: center;
      font-size: 2rem;
      font-weight: bold;
      letter-spacing: 2px;
    }
    nav {
      max-width: 800px;
      margin: 20px auto;
      display: flex;
      justify-content: center;
      gap: 20px;
    }
    nav a {
      color: #4a90e2;
      text-decoration: none;
      font-weight: 600;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      margin: 20px auto;
      max-width: 800px;
    }
    h2 {
      color: #4a90e2;
      border-bottom: 2px solid #4a90e2;
      padding-bottom: 5px;
    }
    ul {
      line-height: 1.6;
    }
    .quiz {
      background: white;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      padding: 20px;
      margin-top: 30px;
    }
    button {
      background: #4a90e2;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
      margin-top: 15px;
    }
    button:hover {
      background: #357ABD;
    }
    .result {
      margin-top: 15px;
      font-weight: bold;
    }
    footer {
      text-align: center;
      margin: 40px 0 20px;
      color: #999;
    }
  </style>
</head>
<body>
  <header>IGCSE Economics Study Hub</header>
  
  <nav>
    <a href="#concepts">Key Concepts</a>
    <a href="#topics">Topics</a>
    <a href="#quiz">Quiz Zone</a>
    <a href="#resources">Resources</a>
  </nav>

  <section id="concepts">
    <h2>Key Concepts</h2>
    <ul>
      <li><strong>Scarcity:</strong> Limited resources vs unlimited wants.</li>
      <li><strong>Opportunity Cost:</strong> The next best alternative you give up.</li>
      <li><strong>Demand:</strong> How much consumers want at a given price.</li>
      <li><strong>Supply:</strong> How much producers are willing to sell at a given price.</li>
      <li><strong>Inflation:</strong> A general increase in prices over time.</li>
      <li><strong>Public Goods vs Private Goods:</strong> Public goods are non-excludable and non-rivalrous, private goods are excludable and rivalrous.</li>
    </ul>
  </section>

  <section id="topics">
    <h2>Topics</h2>
    <ul>
      <li><strong>Basic Economic Problem</strong> - Scarcity and choice.</li>
      <li><strong>Demand and Supply</strong> - Law of demand, supply curve.</li>
      <li><strong>Market Structures</strong> - Perfect competition, monopoly.</li>
      <li><strong>Government Intervention</strong> - Taxes, subsidies, price controls.</li>
      <li><strong>International Trade</strong> - Benefits and barriers.</li>
    </ul>
  </section>

  <section id="quiz" class="quiz">
    <h2>Quick Quiz</h2>
    <p>What does 'opportunity cost' mean?</p>
    <input type="text" id="answer" placeholder="Your answer here..." />
    <button onclick="checkAnswer()">Check Answer</button>
    <p class="result" id="result"></p>
  </section>

  <section id="resources">
    <h2>Resources</h2>
    <ul>
      <li><a href="https://www.bbc.co.uk/bitesize/subjects/zpsvr82" target="_blank">BBC Bitesize Economics</a></li>
      <li><a href="https://qualifications.pearson.com/en/qualifications/edexcel-international-gcses-and-edexcel-certificates/international-gcse-economics-2017.html" target="_blank">Edexcel IGCSE Economics Official</a></li>
      <li><a href="https://www.youtube.com/@EconomicsExplained" target="_blank">Economics Explained (YouTube)</a></li>
    </ul>
  </section>

  <footer>
    Made with ❤️ by Your Bestie Swetha
  </footer>

  <script>
    function checkAnswer() {
      const userAnswer = document.getElementById('answer').value.toLowerCase();
      const result = document.getElementById('result');
      const correctAnswers = [
        'the next best alternative',
        'next best alternative',
        'what you give up',
        'the alternative you give up'
      ];

      if (correctAnswers.some(ans => userAnswer.includes(ans))) {
        result.textContent = '🔥 Correct! Opportunity cost is the next best alternative you give up.';
        result.style.color = 'green';
      } else {
        result.textContent = '❌ Not quite, try again!';
        result.style.color = 'red';
      }
    }
  </script>
</body>
</html>
