# - <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Login</title>
    <style>
        body {
            font-family: Arial, serif;
            margin: 0;
            padding: 0;
            background: url('bghomepage.png') no-repeat center center fixed;
            background-size: cover; /* Adjust the size of the background */
            background-position: center top;
        }

        .container {
            max-width: 600px;
            margin: 150px auto; /* Move the box lower */
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9); /* Slightly transparent background */
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border: 5px solid steelblue; /* Add border */
        }

        .welcome-text {
            font-size: 24px;
            text-align: center;
            color: steelblue; /* Set text color to steelblue */
            animation: bounce 1s infinite alternate; /* Bounce animation */
            margin-bottom: 20px; /* Space below the welcome text */
        }

        @keyframes bounce {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-20px); /* Bounce upward */
            }
        }

        label {
            display: block;
            margin-bottom: 10px;
            font-weight: bold;
            color: steelblue; /* Label color */
        }

        input[type="text"], input[type="password"] {
            width: 100%; /* Full width */
            padding: 10px;
            margin-bottom: 20px; /* Space below each input */
            border: 3px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box; /* Ensure padding doesn't affect width */
        }

        .form-field {
            text-align: center; /* Center the form buttons */
            margin-top: 20px; /* Add margin to move the button lower */
        }

        button, input[type="submit"], input[type="button"] {
            padding: 10px 20px;
            background-color: steelblue; 
            color: #fff;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            margin: 20px auto; /* Add margin between buttons and center the button */
            width: 150px; /* Adjust button width */
            display: block; /* Ensure the button is centered */
        }

        button:hover, input[type="submit"]:hover, input[type="button"]:hover {
            background-color: darkblue; 
        }

        .btn-steelblue {
            background-color: steelblue;
            border-color: steelblue;
            color: #fff;
            padding: 10px 20px;
            border-radius: 12px;
            text-decoration: none;
            display: inline-block;
        }

        .btn-steelblue:hover {
            background-color: darkblue;
            border-color: darkblue;
        }

        .signup-container {
            text-align: center; /* Center the text and button */
            margin-top: 20px; /* Add margin to move the section lower */
        }

        .signup-container p {
            margin: 10px 0; /* Margin for the paragraph */
        }

        .error-message {
            color: red;
            text-align: center;
            margin-top: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="welcome-text">
            <h2>Welcome!</h2>
        </div>
        <form action="loginparcel0.php" method="post">
            <label for="recipientID">ID:</label>
            <input type="text" id="recipientID" name="recipientID" required><br>
            <label for="pass">Password:</label>
            <input type="password" id="pass" name="pass" required><br>
            <?php if (!empty($error_message)): ?>
                <div class="error-message"><?php echo $error_message; ?></div>
            <?php endif; ?>
            <div class="form-field">
                <button type="submit" name="Submit"><b>Login</b></button><br>
            </div>
        </form>
        <div class="signup-container">
            <p><b>Don't have an account yet?</b></p><br>
            <a href="registerparcel.php" class="btn-steelblue"><b>Sign up</b></a><br>
        </div>
    </div>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Login</title>
    <style>
        body {
            font-family: Arial, serif;
            margin: 0;
            padding: 0;
            background: url('bghomepage.png') no-repeat center center fixed;
            background-size: cover; /* Adjust the size of the background */
            background-position: center top;
        }

        .container {
            max-width: 600px;
            margin: 150px auto; /* Move the box lower */
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9); /* Slightly transparent background */
			border: 10px solid #056793;
            border-radius: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .welcome-text {
            font-size: 24px;
            text-align: center;
            color: steelblue; /* Set text color to steelblue */
            animation: bounce 1s infinite alternate; /* Bounce animation */
            margin-bottom: 20px; /* Space below the welcome text */
        }

        @keyframes bounce {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-20px); /* Bounce upward */
            }
        }

        label {
            display: block;
            margin-bottom: 10px;
            font-weight: bold;
            color: steelblue; /* Label color */
        }

        input[type="text"], input[type="password"] {
            width: 100%; /* Full width */
            padding: 10px;
            margin-bottom: 20px; /* Space below each input */
            border: 3px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box; /* Ensure padding doesn't affect width */
        }

        .form-field {
            text-align: center; /* Center the form buttons */
            margin-top: 20px; /* Add margin to move the button lower */
        }

        button, input[type="submit"], input[type="button"] {
            padding: 10px 20px;
            background-color: steelblue; 
            color: #fff;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            margin: 20px auto; /* Add margin between buttons and center the button */
            width: 120px; /* Adjust button width */
            display: block; /* Ensure the button is centered */
			font-weight:bold;
        }

        button:hover, input[type="submit"]:hover, input[type="button"]:hover {
            background-color:  #056793;
        }

        .btn-steelblue {
            background-color: steelblue;
            border-color: steelblue;
            color: #fff;
            padding: 10px 20px;
            border-radius: 12px;
            text-decoration: none;
            display: inline-block;
        }

        .btn-steelblue:hover {
            background-color:#056793;
            border-color: darkblue;
        }

        .signup-container {
            text-align: center; /* Center the text and button */
            margin-top: 20px; /* Add margin to move the section lower */
        }

        .signup-container p {
            margin: 10px 0; /* Margin for the paragraph */
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="welcome-text">
            <h2>Welcome!</h2>
        </div>
        <form action="loginparcel0.php" method="post">
            <label for="recipientID">ID:</label>
            <input type="text" id="recipientID" name="recipientID" required><br>
            <label for="pass">Password:</label>
            <input type="password" id="pass" name="pass" required><br>
            <div class="form-field">
                <button type="submit" name="Submit"><b>Login</b></button><br>
            </div>
        </form>
        <div class="signup-container">
            <p><b>Don't have an account yet?</b></p><br>
            <a href="registerparcel.php" class="btn-steelblue"><b>Sign up</b></a><br>
        </div>
    </div>
</body>
</html>
