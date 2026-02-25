<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Dramatic Queen ❤️</title>

<style>
body {
    margin: 0;
    padding: 0;
    font-family: 'Georgia', serif;
    background: linear-gradient(270deg, #ff4e50, #fc913a, #f9d423, #ff4e50);
    background-size: 800% 800%;
    animation: gradientBG 15s ease infinite;
    color: white;
    text-align: center;
    overflow-x: hidden;
}

@keyframes gradientBG {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
}

.container {
    padding: 50px 20px;
}

h1 {
    font-size: 3em;
    margin-bottom: 10px;
    animation: fadeIn 3s ease-in-out;
}

/* Typing Animation */
.typing {
    border-right: 3px solid white;
    white-space: nowrap;
    overflow: hidden;
    display: inline-block;
    animation: typing 4s steps(30,end), blink .7s infinite;
}

@keyframes typing {
    from { width: 0 }
    to { width: 100% }
}

@keyframes blink {
    50% { border-color: transparent }
}

p {
    font-size: 1.3em;
    max-width: 800px;
    margin: 20px auto;
    line-height: 1.6;
}

.shayari {
    margin-top: 40px;
    font-style: italic;
    font-size: 1.4em;
}

button {
    background: white;
    color: #ff4e50;
    border: none;
    padding: 15px 30px;
    font-size: 1.2em;
    border-radius: 30px;
    cursor: pointer;
    margin-top: 30px;
    transition: 0.3s;
    position: relative;
}

button:hover {
    background: #ff4e50;
    color: white;
    transform: scale(1.1);
}

.hidden {
    display: none;
    margin-top: 30px;
    font-size: 1.5em;
    font-weight: bold;
}

#countdown {
    font-size: 1.5em;
    margin-top: 20px;
    font-weight: bold;
}

/* Floating Hearts */
.heart {
    position: fixed;
    bottom: -10px;
    font-size: 20px;
    animation: floatUp 6s linear infinite;
}

@keyframes floatUp {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-100vh); opacity: 0; }
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}

footer {
    margin-top: 50px;
    padding: 20px;
    font-size: 1em;
    background: rgba(0,0,0,0.3);
}
</style>
</head>

<body>

<div class="container">

<h1>
To My Long Distance Drama Queen ❤️ <br>
<span class="typing">Kausar Qureshi 💖</span>
</h1>

<p>
Yes… I made an entire website just to irritate you lovingly 😌  
Because texting “I miss you” is too normal for us.  
We are long distance… but my drama travels faster than the internet.
</p>

<h2>Countdown Until We Meet 💕</h2>
<div id="countdown"></div>

<p>
Even if there are miles between us,  
my heart still annoys you in real-time.  
And honestly?  
You’re stuck with me forever.
</p>

<div class="shayari">
❤️ Emotional Shayari ❤️ <br><br>
"Door rehkar bhi tum meri sabse kareeb ho,<br>
Meri har dua ka tum hi naseeb ho.<br>
Yeh faasle sirf jism tak seemit hain,<br>
Meri rooh ka tum hi habeeb ho."
</div>

<div class="shayari">
💌 Romantic Shayari 💌 <br><br>
"Tum door ho par ehsaas wahi hai,<br>
Har raat tumhara hi khwaab sahi hai.<br>
Kabhi toh milenge bina screen ke hum,<br>
Aur us din waqt ko bhi rukna padega wahi hai."
</div>

<div class="shayari">
🌙 Long Distance Shayari 🌙 <br><br>
"Yeh dooriyan bhi kya kamaal karti hain,<br>
Mohabbat ko aur bhi bemisaal karti hain.<br>
Milne ki bechaini jab had se badh jaaye,<br>
Tab har dhadkan sirf tumhara naam leti hai."
</div>

<button onclick="showMessage()">Yes I Miss You ❤️</button>
<button id="noBtn">No 😏</button>

<div id="secretMessage" class="hidden">
See? I knew it.  
You miss me more than I miss you.  
And that's scientifically proven.  
(No arguments allowed 😎❤️)
</div>

</div>

<footer>
Conclusion:<br><br>
Distance is temporary.  
Drama is permanent.  
Love is infinite.  
And you… are my forever irritation, my peace, my home. ❤️
</footer>

<script>
// Secret message
function showMessage() {
    document.getElementById("secretMessage").style.display = "block";
}

// Countdown Timer (CHANGE DATE HERE)
var countDownDate = new Date("March 30, 2026 00:00:00").getTime();

var x = setInterval(function() {
    var now = new Date().getTime();
    var distance = countDownDate - now;

    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));

    document.getElementById("countdown").innerHTML =
    days + " Days " + hours + " Hours " + minutes + " Minutes ❤️";

    if (distance < 0) {
        clearInterval(x);
        document.getElementById("countdown").innerHTML = "Finally Together ❤️";
    }
}, 1000);

// Running No Button
var noBtn = document.getElementById("noBtn");
noBtn.addEventListener("mouseover", function() {
    var x = Math.random() * (window.innerWidth - 100);
    var y = Math.random() * (window.innerHeight - 50);
    noBtn.style.position = "absolute";
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});

// Floating Hearts
function createHeart() {
    var heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    heart.style.animationDuration = Math.random() * 3 + 3 + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 6000);
}

setInterval(createHeart, 500);

</script>

</body>
</html>
