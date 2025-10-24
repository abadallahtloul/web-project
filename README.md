[بروجيكت الويب جزء 5 p1.html](https://github.com/user-attachments/files/23128637/5.p1.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Adoption Model</title>
</head>
<body>

  <h2>Adoption</h2>
  <p>Please fill in the following information to complete the adoption request:</p>

  <form id="adoptForm">
  
    <label for="name">Full Name:</label><br>
    <input type="text" id="name" name="name" required minlength="3"><br><br>

    
    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email" required><br><br>

    
    <label for="animal">The type of animal you want to adopt:</label><br>
    <input type="text" id="animal" name="animal" required><br><br>

 
    <label for="reason">The reason for adoption:</label><br>
    <textarea id="reason" name="reason" required minlength="10"></textarea><br><br>

    
    <label for="phone">Phone number:</label><br>
    <input type="tel" id="phone" name="phone" pattern="[0-9]{10}" placeholder="مثال: 0501234567" required><br><br>

   
    <input type="submit" value="Submit Request">
  </form>

 
  <p id="successMessage" style="display:none; color:green;">
    ✅ The adoption request has been sent successfully! Thank you for contacting us. ❤️
  </p>

  <script>
    const form = document.getElementById("adoptForm");
    const success = document.getElementById("successMessage");

    form.addEventListener("submit", function(event) {
      event.preventDefault(); 
      success.style.display = "block"; 
      form.reset(); 
    });
  </script>

</body>
</html>
