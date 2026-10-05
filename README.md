<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy 18th 🎀</title>

<!-- 🌸 FONT ESTETIK -->
<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400&display=swap" rel="stylesheet">

<style>
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: #ffeef2;
    color: #444;
    text-align: center;
}

/* CONTAINER */
.container {
    padding: 30px;
}

/* NAMA ESTETIK */
.name {
    font-family: 'Great Vibes', cursive;
    font-size: 42px;
    color: #ff6f91;
    margin-top: 10px;
}

/* TITLE */
h1 {
    color: #ff8fab;
}

/* FOTO GANTUNG */
.gallery {
    display: flex;
    justify-content: center;
    gap: 15px;
    flex-wrap: wrap;
    margin-top: 20px;
}

.photo {
    background: white;
    padding: 10px;
    border-radius: 10px;
    width: 120px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transform: rotate(-3deg);
    position: relative;
}

.photo:nth-child(even){
    transform: rotate(3deg);
}

.photo::before {
    content: "";
    width: 2px;
    height: 40px;
    background: #bbb;
    position: absolute;
    top: -40px;
    left: 50%;
}

.photo img {
    width: 100%;
    border-radius: 5px;
}

/* MESSAGE */
.message {
    background: white;
    margin: 30px auto;
    padding: 20px;
    max-width: 500px;
    border-radius: 15px;
    line-height: 1.7;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    display: none;
}

/* BUTTON */
button {
    padding: 10px 20px;
    border: none;
    border-radius: 20px;
    background: #ff8fab;
    color: white;
    cursor: pointer;
    margin-top: 15px;
}
</style>
</head>

<body>

<div class="container">

<h1>🎀 Happy 18th Birthday 🎀</h1>

<div class="name">Nur Nayla Sari Putri</div>

<button onclick="showMessage()">Open Your Gift 🎁</button>

<!-- 🎵 MUSIC -->
<audio autoplay loop>
    <source src="music.mp3" type="audio/mpeg">
</audio>

<!-- 🖼️ FOTO GANTUNG -->
<div class="gallery">
    <div class="photo"><img src="1.jpg"></div>
    <div class="photo"><img src="2.jpg"></div>
    <div class="photo"><img src="3.jpg"></div>
    <div class="photo"><img src="4.jpg"></div>
</div>

<!-- 💌 PESAN -->
<div id="msg" class="message"></div>

</div>

<script>

function showMessage(){
    let name = "Nur Nayla Sari Putri";

    document.getElementById("msg").style.display = "block";

    document.getElementById("msg").innerHTML =
    "Happy 18th Birthday, <b>" + name + "</b> 🎂💗<br><br>" +

    "Today is a very special day... not just because it's your birthday, " +
    "but because you are officially stepping into a new chapter of life.<br><br>" +

    "18 is not just a number. It’s a symbol of growth, strength, and new beginnings. " +
    "You’ve come so far, and I’m so proud of the person you are becoming.<br><br>" +

    "Through all the ups and downs, you stayed strong. " +
    "You kept going, you kept smiling, and you never gave up.<br><br>" +

    "I hope this new chapter brings you endless happiness, " +
    "beautiful memories, and dreams that slowly come true.<br><br>" +

    "Always remember: you are loved, you are important, and you are enough.<br><br>" +

    "💖 Happy Birthday once again, " + name + " 💖<br>" +
    "✨ You deserve all the happiness in the world ✨";
}

</script>

</body>
</html>
