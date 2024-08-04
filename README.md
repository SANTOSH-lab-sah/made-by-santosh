<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Friendship Day Wish</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            color: #333;
        }
        h1 {
            color: #ff4500;
        }
    </style>
</head>
<body>

    <h1 id="wishMessage">Happy Friendship Day, <span id="friendName"></span>!</h1>

    <script>
        const urlParams = new URLSearchParams(window.location.search);
        const friendName = urlParams.get('name');

        if(friendName) {
            document.getElementById('friendName').textContent = friendName;
        } else {
            document.getElementById('wishMessage').textContent = 'Happy Friendship Day!';
        }
    </script>

</body>
</html>
