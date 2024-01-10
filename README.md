<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Date Invitation</title>
    <style>
        body {
            background-color: #f7f7f7;
            text-align: center;
            font-family: 'Arial', sans-serif;
        }

        h1 {
            color: #ff4081;
        }

        p {
            color: #333;
        }

        button {
            background-color: #ff4081;
            color: #fff;
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            cursor: pointer;
        }

        #response {
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            color: #333;
        }

        #cute-message, #sad-message {
            display: none;
        }
    </style>
</head>
<body>
    <h1>Hey Darling</h1>
    <p>Would you like to go on a special date with me on 17th?</p>
    
    <button onclick="acceptInvitation()">Yes, I'd love to!</button>
    <button onclick="rejectInvitation()">Sorry, not this time.</button>

    <div id="response"></div>
    <div id="cute-message">Yay! Can't wait for our special date! lets have a lot of food😊</div>
    <div id="sad-message">Oh, thats sad 😔</div>

    <script>
        function acceptInvitation() {
            document.getElementById('response').innerHTML = 'Your response: Yes';
            document.getElementById('cute-message').style.display = 'block';
            document.getElementById('sad-message').style.display = 'none';
        }

        function rejectInvitation() {
            document.getElementById('response').innerHTML = 'Your response: No';
            document.getElementById('sad-message').style.display = 'block';
            document.getElementById('cute-message').style.display = 'none';
        }
    </script>
</body>
</html>


