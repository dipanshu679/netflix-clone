<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Netflix Clone</title>
  <link rel="stylesheet" href="style.css" />
</head>
<style>
  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: black;
  color: white;
  height: 3112px;
}

.back {
  min-height: 116.3vh;
  background: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.8) 0%,
      rgba(0, 0, 0, 0.2) 40%,
      rgba(0, 0, 0, 0.8) 100%
    ),
    url('image___netflix.jpg') no-repeat center center/cover;
  display: flex;
  flex-direction: column;
}

header {
  max-width: 1200px;
  width: 100%;
  margin-left:80px;
  padding: px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo img {
  height: 120px;
  width: 200px;
}

nav form {
  display: flex;
  gap: 10px;
  align-items: center;
}

.language-selector {
  display: flex;
  align-items: center;
  gap: 8px;
  border: 1px solid white;
  padding: 6px 10px;
  border-radius: 3px;
  background-color: transparent;
  color: white;
}

.language-selector ion-icon {
  font-size: 18px;
  color: white;
}

.language-selector select {
  background-color: black;
  color: white;
  border: none;
  font-size: 14px;
  outline: none;
  cursor: pointer;
}

/* Dropdown ke options ke liye styling */
.language-selector select option {
  background-color:white;
  color: black;
}

button {
  padding: 6px 14px;
  background-color: red;
  color: white;
  border: none;
  border-radius: 3px;
  font-weight: bold;
  cursor: pointer;
  font-size: 14px;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: darkred;
}

@media (max-width: 768px) {
  header {
    flex-direction: column;
    gap: 20px;
    text-align: center;
  }

  nav form {
    flex-direction: column;
    gap: 10px;
  }
}

</style>
<body>
  <div class="back">
    <header>
      <div class="logo">
        <img src="Netflix_Logo_CMYK.png" alt="Netflix Logo" />
      </div>
      <nav>
        <form>
          <div class="language-selector">
            <ion-icon name="language"></ion-icon>
            <select>
              <option value="en">English</option>
              <option value="hi">हिन्दी</option>
            </select>
          </div>
          <button type="button">Sign In</button>
        </form>
      </nav>
    </header>
  </div>

  <!-- Ionicons scripts -->
  <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
  <script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>

</html>
