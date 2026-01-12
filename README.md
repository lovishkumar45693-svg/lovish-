
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Student Login Page</title>

    <!-- ===== CSS START ===== -->
    <style>
        body {
            background: linear-gradient(to right, #74ebd5, #9face6);
            font-family: Arial, sans-serif;
        }

        .login-box {
            width: 320px;
            background: white;
            margin: 120px auto;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0,0,0,0.3);
            text-align: center;
        }

        .login-box h2 {
            margin-bottom: 20px;
            color: #333;
        }

        .login-box input {
            width: 90%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid gray;
            border-radius: 5px;
        }

        .login-box button {
            width: 95%;
            padding: 10px;
            background-color: #0066cc;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }

        .login-box button:hover {
            background-color: #004d99;
        }

        #message {
            margin-top: 15px;
            font-weight: bold;
        }
    </style>
    <!-- ===== CSS END ===== -->
</head>

<body>

    <div class="login-box">
        <h2>Student Login</h2>

        <input type="text" id="username" placeholder="Enter Username">
        <input type="password" id="password" placeholder="Enter Password">

        <button onclick="login()">Login</button>

        <p id="message"></p>
    </div>

    <!-- ===== JAVASCRIPT START ===== -->
    <script>
        function login() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            if (username === "student" && password === "12345") {
                document.getElementById("message").style.color = "green";
                document.getElementById("message").innerHTML =
                    "Login Successful! Welcome Student 🎉";
            } else {
                document.getElementById("message").style.color = "red";
                document.getElementById("message").innerHTML =
                    "Invalid Username or Password ❌";
            }
        }
    </script>
    <!-- ===== JAVASCRIPT END ===== -->

</body>
</html>
