# Classic Admin Login Page

A simple admin dashboard login interface built with HTML, CSS, and a secure login form simulation.

## Features

- Classic admin dashboard design  
- Secure username/password login  
- Prefilled demo credentials (Username: admin / Password: admin.123)  
- Responsive and minimal CSS styling  

## Demo Code

```
<div align="center">

  <!-- Classic Admin Login Page -->
  <form onsubmit="return validateLogin(event)" style="width: 320px; padding: 20px; border: 1px solid #ccc; background: #f9f9f9; border-radius: 8px;">
    <h2>Admin Login</h2>
    <label for="username">Username:</label><br>
    <input type="text" id="username" name="username" placeholder="Enter your username" required style="width: 100%;"><br><br>
    <label for="password">Password:</label><br>
    <input type="password" id="password" name="password" placeholder="Enter your password" required style="width: 100%;"><br><br>
    <button type="submit" style="width: 100%; background-color: #007BFF; color: white; padding: 10px; border: none; border-radius: 4px;">Login</button>
    <p id="message" style="color:red; margin-top:10px;"></p>
  </form>

</div>

<script>
function validateLogin(event) {
  event.preventDefault();
  const username = document.getElementById('username').value.trim();
  const password = document.getElementById('password').value.trim();
  const message = document.getElementById('message');
  
  if (username === 'admin' && password === 'admin.123') {
    message.style.color = 'green';
    message.textContent = 'Login successful! Redirecting...';
    setTimeout(() => { window.location.href = '#dashboard'; }, 1000);
  } else {
    message.textContent = 'Invalid username or password';
  }
}
</script>
```

## contact: adishhhh9@gmail.com

## License

This project is open-source and free for any use or modification.
```

***

Would you like me to include a mock “Admin Dashboard” page that appears after successful login?
