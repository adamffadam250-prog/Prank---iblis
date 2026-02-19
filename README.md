<!DOCTYPE html>
<html>
<head>
    <title>Loading...</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            background-color: black;
            color: white;
            text-align: center;
            font-family: Arial;
            margin-top: 200px;
            transition: 0.2s;
        }

        button {
            padding: 20px 40px;
            font-size: 20px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<h1 id="text">Tap untuk masuk 🗿</h1>
<button onclick="startPrank()">MASUK</button>

<audio id="sound">
    <source src="suara.mp3" type="audio/mpeg">
</audio>

<script>
function startPrank() {
    var audio = document.getElementById("sound");

    audio.volume = 1.0;
    audio.play();

    document.body.style.backgroundColor = "red";
    document.getElementById("text").innerText = "KENAAAAA 😈💀";
    document.querySelector("button").style.display = "none";

    if (document.documentElement.requestFullscreen) {
        document.documentElement.requestFullscreen();
    }
}
</script>

</body>
</html>
