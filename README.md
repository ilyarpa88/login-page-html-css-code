# login-page-html-css-code
I creat a normality loading page with html&amp;css 
/*html*/
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Loading Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<link rel="stylesheet" href="first.css">
<div class="loader-container">
  <div class="loader"></div>
  <p>Loading...</p>
</div>

<script>
  // Redirect to the next page after 3 seconds
  setTimeout(function() {
    window.location.href = 'web.html'; // Replace 'other-page.html' with your actual target page URL
  }, 3000); // 3 seconds
</script>
 
</body>
</html>

/*css*/

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.loader-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.loader {
  border: 8px solid #f3f3f3;
  border-top: 8px solid #3498db;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  animation: spin 1s linear infinite;
  margin-bottom: 20px;
}

@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

p {
  font-size: 18px;
  color: #555;
}
