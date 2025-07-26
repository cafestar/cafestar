<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Coffee Star Menu</title>
<style>
  body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #fdfdfd;
    margin: 0;
    padding: 0;
  }
  h1 {
    font-size: 24px;
    margin-top: 20px;
  }
  #menu-container img {
    max-width: 90%;
    height: auto;
    margin: 15px auto;
    display: block;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.15);
  }
  button {
    background-color: #6f4e37;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 6px;
    font-size: 16px;
    cursor: pointer;
    margin: 15px;
  }
  button:hover {
    background-color: #8b5e3c;
  }
</style>
</head>
<body>
  <div>
    <img src="https://lottie.host/1ff9a3a0-1234-4f00-9abc-coffee-cup.gif" alt="coffee animation" width="120">
    <h1>hi🖐🏼<br>Welcome to Coffee Star</h1>
  </div>

  <div id="menu-container">
    <img id="menu-image" src="english-menu.jpg" alt="English Menu">
  </div>

  <button onclick="switchMenu()">مشاهده منوی فارسی</button>

<script>
  let englishMenu = "english-menu.jpg";
  let persianMenu = "persian-menu.jpg";
  let showingEnglish = true;
  function switchMenu(){
    let img = document.getElementById("menu-image");
    if(showingEnglish){
      img.src = persianMenu;
      document.querySelector("button").innerText = "View English Menu";
      showingEnglish = false;
    } else {
      img.src = englishMenu;
      document.querySelector("button").innerText = "مشاهده منوی فارسی";
      showingEnglish = true;
    }
  }
</script>
</body>
</html>
