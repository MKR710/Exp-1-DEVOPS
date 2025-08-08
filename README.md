<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Registration Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .container {
      background: #ffffff;
      padding: 30px 40px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
      width: 100%;
      max-width: 500px;
    }

    .container h2 {
      text-align: center;
      margin-bottom: 25px;
    }

    .form-group {
      margin-bottom: 15px;
    }

    .form-group label {
      display: block;
      margin-bottom: 6px;
      font-weight: bold;
    }

    .form-group input,
    .form-group textarea {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .gender-group {
      display: flex;
      gap: 15px;
      margin-top: 5px;
    }

    .gender-group label {
      font-weight: normal;
    }

    .register-btn {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }

    .register-btn button {
      padding: 10px 30px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }

    .register-btn button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Registration Form</h2>
    <form>
      <div class="form-group">
        <label for="fname">First Name</label>
        <input type="text" id="fname" name="fname" required>
      </div>

      <div class="form-group">
        <label for="lname">Last Name</label>
        <input type="text" id="lname" name="lname" required>
      </div>

      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
      </div>

      <div class="form-group">
        <label for="mobile">Mobile</label>
        <input type="tel" id="mobile" name="mobile" required pattern="[0-9]{10}">
      </div>

      <div class="form-group">
        <label for="address">Address</label>
        <textarea id="address" name="address" rows="3" required></textarea>
      </div>

      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" name="password" required>
      </div>

      <div class="form-group">
        <label>Gender</label>
        <div class="gender-group">
          <label><input type="radio" name="gender" value="Male" required> Male</label>
          <label><input type="radio" name="gender" value="Female"> Female</label>
          <label><input type="radio" name="gender" value="Other"> Other</label>
        </div>
      </div>

      <div class="register-btn">
        <button type="submit">Register</button>
      </div>
    </form>
  </div>
</body>
</html>
