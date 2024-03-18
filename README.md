<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Knowledge Challenge Series: Clothes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
        }
        header {
            background-color: rgba(255, 255, 255, 0.7);
            padding: 20px;
            text-align: center;
        }
        section {
            padding: 20px;
            margin: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            text-align: center;
        }
        h1, h2 {
            color: #333;
        }
        p {
            line-height: 1.6;
        }
        .welcome {
            background-image: url('clo.jpg');
            background-size: cover;
            background-position: center;
            color: darkred;
        }
        .quiz {
            background-image: url('ques.jpg');
            background-size: cover;
            background-position: center;
            color: black;
        }
        .thank-you {
            background-image: url('thanks.jpg');
            background-size: cover;
            background-position: center;
            color: #000;
            text-transform: uppercase;
            font-size: 36px;
        }
        .quiz button {
            background-color: #333;
            color: black;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .quiz input[type="submit"] {
            background-color: #333;
            color: brown;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1 class="welcome" style="color: purple;">Knowledge Challenge Series: Clothes</h1>
    </header>
    <section class="welcome">
        <h2>Welcome to the Clothes Knowledge Challenge!</h2>
        <p>Test your knowledge about clothes by playing our quiz.</p>
        <p>Click the button below to start the quiz.</p>
        <button onclick="startQuiz()">Start Quiz</button>
    </section>

    <section class="quiz" id="quizSection" style="display: none;">
        <h2>Quiz on Clothes</h2>
        <form id="quizForm" action="#" onsubmit="submitQuiz(); return false;">
            <div class="question">
                <label for="q1">Question 1: What is the traditional Japanese robe called?</label><br>
                <input type="radio" name="q1" value="a"> Kimono<br>
                <input type="radio" name="q1" value="b"> Sari<br>
                <input type="radio" name="q1" value="c"> Hanbok<br>
                <input type="radio" name="q1" value="d"> Dashiki<br>
            </div>
            <div class="question">
                <label for="q2">Question 2: What is the name of the fabric commonly used to make jeans?</label><br>
                <input type="radio" name="q2" value="a"> Polyester<br>
                <input type="radio" name="q2" value="b"> Denim<br>
                <input type="radio" name="q2" value="c"> Cotton<br>
                <input type="radio" name="q2" value="d"> Wool<br>
            </div>
            <div class="question">
                <label for="q3">Question 3: Who is the famous fashion designer known for the little black dress?</label><br>
                <input type="radio" name="q3" value="a"> Coco Chanel<br>
                <input type="radio" name="q3" value="b"> Gianni Versace<br>
                <input type="radio" name="q3" value="c"> Christian Dior<br>
                <input type="radio" name="q3" value="d"> Ralph Lauren<br>
            </div>
            <input type="submit" value="Submit Quiz">
        </form>
    </section>

    <section class="thank-you" id="thankYouSection" style="display: none;">
        <h2>Thank you for taking the quiz!</h2>
        <p>We appreciate your participation.</p>
    </section>

    <script>
        function startQuiz() {
            document.getElementById("quizSection").style.display = "block";
        }

        function submitQuiz() {
            // Process the quiz submission here
            // For demonstration purposes, simply display the thank you message
            document.getElementById("quizSection").style.display = "none";
            document.getElementById("thankYouSection").style.display = "block";
        }
    </script>
</body>
</html>
