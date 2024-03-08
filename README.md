<!DOCTYPE html>
<html>
<head>
    <title>Login page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f29a;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 300px;
            padding: 16px;
            background-color: #fff;
            margin: 75px auto;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1 {
            text-align: center;
            margin-top: 0;
        }
        input[type="text"], input[type="password"], input[type="email"] {
            width: 100%;
            padding: 10px;
            margin-top: 8px;
            margin-bottom: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 16px;
        }
        input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
        .form-switch {
            text-align: center;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1><b>login</b></h1>
        <form id="login-form" action="/login" method="post">
            <label for="login-username">Username:</label>
            <input type="text" id="login-username" name="username" required>
            <label for="login-password">Password:</label>
            <input type="password" id="login-password" name="password" required>
            <input type="submit" value="Log In">
        </form>
        <div class="form-switch">
            <span>Don't have an account?</span>
            <button onclick="switchForm()">Sign Up</button>
        </div>
        <form id="signup-form" action="/signup" method="post" style="display: none;">
            <label for="signup-username">Username:</label>
            <input type="text" id="signup-username" name="username" required>
            <label for="signup-email">Email:</label>
            <input type="email" id="signup-email" name="email" required>
            <label for="signup-password">Password:</label>
            <input type="password" id="signup-password" name="password" required>
            <input type="submit" value="Sign Up">
        </form>
    </div>

</body>
</html>

