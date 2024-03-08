<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SpaceX Signup</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #0a0a23;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            background-color: #2e2e5f;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
            max-width: 100%;
        }

        h2 {
            margin-top: 0;
            text-align: center;
            color: #fff;
        }

        input[type="text"],
        input[type="password"] {
            width: 100%;
            padding: 10px;
            margin: 8px 0;
            box-sizing: border-box;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        input[type="submit"] {
            width: 100%;
            background-color: #007bff;
            color: white;
            padding: 14px 20px;
            margin: 8px 0;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        input[type="submit"]:hover {
            background-color: #0056b3;
        }

        .spacex-logo {
            display: block;
            margin: 0 auto;
            width: 150px;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/SpaceX-Logo-Xonly.svg/2560px-SpaceX-Logo-Xonly.svg.png" alt="SpaceX Logo" class="spacex-logo">
        <h2>Signup</h2>
        <form action="/signup" method="post">
            <label for="username" style="color: #fff;">Username:</label>
            <input type="text" id="username" name="username" required>

            <label for="password" style="color: #fff;">Password:</label>
            <input type="password" id="password" name="password" required>

            <label for="confirm_password" style="color: #fff;">Confirm Password:</label>
            <input type="password" id="confirm_password" name="confirm_password" required>

            <input type="submit" value="Signup">
        </form>
    </div>
</body>
</html>
