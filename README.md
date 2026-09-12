 # Birthdaywebsite.-
```html
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport"
      content="width=device-width, initial-scale=1.0,
               maximum-scale=1.0, user-scalable=no">

<title>Happy Birthday ❤️</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html,body{
  width:100%;
  min-height:100%;
  overflow-x:hidden;
  font-family:Arial, sans-serif;
  background:#fff0f6;
}

body{
  color:#4a1830;
}

/* Main */
.container{
  min-height:100vh;
  width:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
  text-align:center;
  position:relative;
  overflow:hidden;
}

/* Top section */
.hero{
  min-height:100vh;
  width:100%;
  padding:70px 20px 40px;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;

  background:
    radial-gradient(circle at 20% 20%, #ffd6e8 0 5%, transparent 6%),
    radial-gradient(circle at 80% 30%, #ffe3ef 0 5%, transparent 6%),
    linear-gradient(180deg,#fff0f7,#ffe0ec);
}

.small{
  font-size:18px;
  letter-spacing:3px;
  color:#d63384;
  margin-bottom:12px;
}

h1{
  font-size:clamp(38px,12vw,70px);
  color:#e91e63;
  line-height:1.05;
  text-shadow:0 4px 12px rgba(233,30,99,.18);
}

.name{
  margin-top:18px;
  font-size:clamp(42px,13vw,75px);
  font-weight:900;
  background:linear-gradient(90deg,#ff4081,#9c27b0,#ff4081);
  background-size:200% auto;
  color:transparent;
  -webkit-background-clip:text;
  background-clip:text;
  animation:nameGlow 3s linear infinite;
}

@keyframes nameGlow{
  to{background-position:200% center;}
}

.message{
  margin-top:22px;
  max-width:500px;
  font-size:18px;
  line-height:1.7;
  color:#6d304c;
}

.cake{
  font-size:75px;
  margin:25px 0 10px;
  animation:cakeBounce 2s ease-in-out infinite;
}

@keyframes cakeBounce{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-10px)}
}

.scroll{
  margin-top:30px;
  color:#c2185b;
  font-size:14px;
  animation:upDown 1.5s infinite;
}

@keyframes upDown{
  50%{transform:translateY(8px)}
}

/* Letter */
.letter-section{
  width:100%;
  padding:70px 18px 100px;
  background:#fff8fb;
}

.letter{
  width:100%;
  max-width:550px;
  margin:auto;
  padding:30px 22px;
  background:#fffdf8;
  border-radius:18px;
  box-shadow:0 12px 35px rgba(120,40,80,.12);
  text-align:left;
  border:1px solid #f7d6e4;
}

.letter-title{
  text-align:center;
  font-size:28px;
  color:#d81b60;
  margin-bottom:25px;
}

.letter p{
  font-size:17px;
  line-height:1.9;
  color:#573044;
  margin-bottom:16px;
}

.signature{
  text-align:right;
  margin-top:25px;
  font-size:18px;
  color:#c2185b;
}

/* Floating balloons */
.balloon{
  position:fixed;
  bottom:-100px;
  width:38px;
  height:50px;
  border-radius:50%;
  opacity:.85;
  z-index:5;
  animation:balloonUp linear infinite;
}

.balloon::after{
  content:"";
  position:absolute;
  width:1px;
  height:65px;
  background:#777;
  top:48px;
  left:50%;
}

.balloon::before{
  content:"";
  position:absolute;
  bottom:-5px;
  left:50%;
  transform:translateX(-50%);
  border-left:5px solid transparent;
  border-right:5px solid transparent;
  border-top:8px solid currentColor;
}

.b1{
  left:8%;
  background:#ff4d6d;
  color:#ff4d6d;
  animation-duration:8s;
}

.b2{
  left:28%;
  width:32px;
  height:43px;
  background:#9c27b0;
  color:#9c27b0;
  animation-duration:10s;
  animation-delay:2s;
}

.b3{
  left:55%;
  background:#ff9800;
  color:#ff9800;
  animation-duration:9s;
  animation-delay:1s;
}

.b4{
  left:78%;
  width:34px;
  height:46px;
  background:#2196f3;
  color:#2196f3;
  animation-duration:11s;
  animation-delay:3s;
}

@keyframes balloonUp{
  0%{
    transform:translateY(0) rotate(-5deg);
  }
  50%{
    transform:translateY(-55vh) rotate(6deg);
  }
  100%{
    transform:translateY(-120vh) rotate(-5deg);
  }
}

/* Falling flowers */
.petal{
  position:fixed;
  top:-30px;
  z-index:4;
  pointer-events:none;
  animation:fall linear infinite;
}

@keyframes fall{
  0%{
    transform:translateY(-30px) rotate(0deg);
    opacity:0;
  }

  10%{
    opacity:1;
  }

  100%{
    transform:translateY(110vh) rotate(360deg);
    opacity:.8;
  }
}

/* Footer */
.footer{
  padding:25px 15px 40px;
  background:#fff8fb;
  color:#a44a6d;
  font-size:14px;
}
</style>
</head>

<body>

<div class="container">

  <!-- BALLOONS -->
  <div class="balloon b1"></div>
  <div class="balloon b2"></div>
  <div class="balloon b3"></div>
  <div class="balloon b4"></div>

  <!-- BIRTHDAY SECTION -->
  <section class="hero">

    <div class="small">✨ TODAY IS YOUR DAY ✨</div>

    <h1>Happy Birthday</h1>

    <!-- এখানে নাম পরিবর্তন করুন -->
    <div class="name">প্রিয় মানুষ ❤️</div>

    <div class="cake">🎂</div>

    <p class="message">
      আজকের এই বিশেষ দিনে তোমার জীবনে
      আসুক অনেক আনন্দ, ভালোবাসা,
      হাসি আর সুন্দর সুন্দর মুহূর্ত। 🌸
      <br><br>
      তোমার প্রতিটি স্বপ্ন পূরণ হোক,
      আর প্রতিটি দিন হয়ে উঠুক
      আজকের দিনের মতোই সুন্দর। 💖
    </p>

    <div class="scroll">
      নিচে আসো... তোমার জন্য আরও কিছু আছে 💌
      <br>↓
    </div>

  </section>

  <!-- LETTER -->
  <section class="letter-section">

    <div class="letter">

      <div class="letter-title">
        💌 তোমার জন্য একটি চিঠি
      </div>

      <p>
        প্রিয়,
      </p>

      <p>
        আজ তোমার জন্মদিন। তাই আজকের দিনটা
        তোমাকে একটু অন্যভাবে মনে করিয়ে দিতে
        চাই—তুমি সত্যিই অনেক বিশেষ একজন মানুষ।
      </p>

      <p>
        জীবনের পথে যত কঠিন সময়ই আসুক,
        তোমার মুখের হাসিটা যেন কখনো হারিয়ে না যায়।
        তোমার ছোট ছোট ইচ্ছেগুলো পূরণ হোক,
        আর তোমার জীবনে সবসময় ভালো মানুষ ও
        সুন্দর মুহূর্তগুলো পাশে থাকুক। 🌷
      </p>

      <p>
        আজ শুধু একটি কথাই বলতে চাই—
        নিজের মতো করে সুন্দর থেকো,
        হাসিখুশি থেকো এবং নিজের স্বপ্নগুলোকে
        কখনো ছেড়ে দিও না।
      </p>

      <p>
        আবারও তোমাকে জানাই
        <strong>শুভ জন্মদিন। 🎂🎉</strong>
      </p>

      <div class="signature">
        অনেক ভালোবাসা ❤️<br>
        তোমার আপনজন
      </div>

    </div>

  </section>

  <div class="footer">
    Made with ❤️ just for you
  </div>

</div>


<script>
/* Lightweight falling petals */
const symbols = ["🌸","🌷","💮","🌺","✿"];

function createPetal(){

  const petal = document.createElement("div");

  petal.className = "petal";
  petal.textContent =
    symbols[Math.floor(Math.random()*symbols.length)];

  petal.style.left =
    Math.random()*100 + "vw";

  petal.style.fontSize =
    (12 + Math.random()*12) + "px";

  petal.style.animationDuration =
    (5 + Math.random()*5) + "s";

  petal.style.animationDelay =
    Math.random()*2 + "s";

  document.body.appendChild(petal);

  setTimeout(()=>{
    petal.remove();
  },10000);
}

/* Only a few petals at a time = smooth on mobile */
setInterval(createPetal,700);
</script>

</body>
</html>
```
```html
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport"
      content="width=device-width, initial-scale=1.0,
               maximum-scale=1.0, user-scalable=no">

<title>Happy Birthday ❤️</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html,body{
  width:100%;
  min-height:100%;
  overflow-x:hidden;
  font-family:Arial, sans-serif;
  background:#fff0f6;
}

body{
  color:#4a1830;
}

/* Main */
.container{
  min-height:100vh;
  width:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
  text-align:center;
  position:relative;
  overflow:hidden;
}

/* Top section */
.hero{
  min-height:100vh;
  width:100%;
  padding:70px 20px 40px;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;

  background:
    radial-gradient(circle at 20% 20%, #ffd6e8 0 5%, transparent 6%),
    radial-gradient(circle at 80% 30%, #ffe3ef 0 5%, transparent 6%),
    linear-gradient(180deg,#fff0f7,#ffe0ec);
}

.small{
  font-size:18px;
  letter-spacing:3px;
  color:#d63384;
  margin-bottom:12px;
}

h1{
  font-size:clamp(38px,12vw,70px);
  color:#e91e63;
  line-height:1.05;
  text-shadow:0 4px 12px rgba(233,30,99,.18);
}

.name{
  margin-top:18px;
  font-size:clamp(42px,13vw,75px);
  font-weight:900;
  background:linear-gradient(90deg,#ff4081,#9c27b0,#ff4081);
  background-size:200% auto;
  color:transparent;
  -webkit-background-clip:text;
  background-clip:text;
  animation:nameGlow 3s linear infinite;
}

@keyframes nameGlow{
  to{background-position:200% center;}
}

.message{
  margin-top:22px;
  max-width:500px;
  font-size:18px;
  line-height:1.7;
  color:#6d304c;
}

.cake{
  font-size:75px;
  margin:25px 0 10px;
  animation:cakeBounce 2s ease-in-out infinite;
}

@keyframes cakeBounce{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-10px)}
}

.scroll{
  margin-top:30px;
  color:#c2185b;
  font-size:14px;
  animation:upDown 1.5s infinite;
}

@keyframes upDown{
  50%{transform:translateY(8px)}
}

/* Letter */
.letter-section{
  width:100%;
  padding:70px 18px 100px;
  background:#fff8fb;
}

.letter{
  width:100%;
  max-width:550px;
  margin:auto;
  padding:30px 22px;
  background:#fffdf8;
  border-radius:18px;
  box-shadow:0 12px 35px rgba(120,40,80,.12);
  text-align:left;
  border:1px solid #f7d6e4;
}

.letter-title{
  text-align:center;
  font-size:28px;
  color:#d81b60;
  margin-bottom:25px;
}

.letter p{
  font-size:17px;
  line-height:1.9;
  color:#573044;
  margin-bottom:16px;
}

.signature{
  text-align:right;
  margin-top:25px;
  font-size:18px;
  color:#c2185b;
}

/* Floating balloons */
.balloon{
  position:fixed;
  bottom:-100px;
  width:38px;
  height:50px;
  border-radius:50%;
  opacity:.85;
  z-index:5;
  animation:balloonUp linear infinite;
}

.balloon::after{
  content:"";
  position:absolute;
  width:1px;
  height:65px;
  background:#777;
  top:48px;
  left:50%;
}

.balloon::before{
  content:"";
  position:absolute;
  bottom:-5px;
  left:50%;
  transform:translateX(-50%);
  border-left:5px solid transparent;
  border-right:5px solid transparent;
  border-top:8px solid currentColor;
}

.b1{
  left:8%;
  background:#ff4d6d;
  color:#ff4d6d;
  animation-duration:8s;
}

.b2{
  left:28%;
  width:32px;
  height:43px;
  background:#9c27b0;
  color:#9c27b0;
  animation-duration:10s;
  animation-delay:2s;
}

.b3{
  left:55%;
  background:#ff9800;
  color:#ff9800;
  animation-duration:9s;
  animation-delay:1s;
}

.b4{
  left:78%;
  width:34px;
  height:46px;
  background:#2196f3;
  color:#2196f3;
  animation-duration:11s;
  animation-delay:3s;
}

@keyframes balloonUp{
  0%{
    transform:translateY(0) rotate(-5deg);
  }
  50%{
    transform:translateY(-55vh) rotate(6deg);
  }
  100%{
    transform:translateY(-120vh) rotate(-5deg);
  }
}

/* Falling flowers */
.petal{
  position:fixed;
  top:-30px;
  z-index:4;
  pointer-events:none;
  animation:fall linear infinite;
}

@keyframes fall{
  0%{
    transform:translateY(-30px) rotate(0deg);
    opacity:0;
  }

  10%{
    opacity:1;
  }

  100%{
    transform:translateY(110vh) rotate(360deg);
    opacity:.8;
  }
}

/* Footer */
.footer{
  padding:25px 15px 40px;
  background:#fff8fb;
  color:#a44a6d;
  font-size:14px;
}
</style>
</head>

<body>

<div class="container">

  <!-- BALLOONS -->
  <div class="balloon b1"></div>
  <div class="balloon b2"></div>
  <div class="balloon b3"></div>
  <div class="balloon b4"></div>

  <!-- BIRTHDAY SECTION -->
  <section class="hero">

    <div class="small">✨ TODAY IS YOUR DAY ✨</div>

    <h1>Happy Birthday</h1>

    <!-- এখানে নাম পরিবর্তন করুন -->
    <div class="name">প্রিয় মানুষ ❤️</div>

    <div class="cake">🎂</div>

    <p class="message">
      আজকের এই বিশেষ দিনে তোমার জীবনে
      আসুক অনেক আনন্দ, ভালোবাসা,
      হাসি আর সুন্দর সুন্দর মুহূর্ত। 🌸
      <br><br>
      তোমার প্রতিটি স্বপ্ন পূরণ হোক,
      আর প্রতিটি দিন হয়ে উঠুক
      আজকের দিনের মতোই সুন্দর। 💖
    </p>

    <div class="scroll">
      নিচে আসো... তোমার জন্য আরও কিছু আছে 💌
      <br>↓
    </div>

  </section>

  <!-- LETTER -->
  <section class="letter-section">

    <div class="letter">

      <div class="letter-title">
        💌 তোমার জন্য একটি চিঠি
      </div>

      <p>
        প্রিয়,
      </p>

      <p>
        আজ তোমার জন্মদিন। তাই আজকের দিনটা
        তোমাকে একটু অন্যভাবে মনে করিয়ে দিতে
        চাই—তুমি সত্যিই অনেক বিশেষ একজন মানুষ।
      </p>

      <p>
        জীবনের পথে যত কঠিন সময়ই আসুক,
        তোমার মুখের হাসিটা যেন কখনো হারিয়ে না যায়।
        তোমার ছোট ছোট ইচ্ছেগুলো পূরণ হোক,
        আর তোমার জীবনে সবসময় ভালো মানুষ ও
        সুন্দর মুহূর্তগুলো পাশে থাকুক। 🌷
      </p>

      <p>
        আজ শুধু একটি কথাই বলতে চাই—
        নিজের মতো করে সুন্দর থেকো,
        হাসিখুশি থেকো এবং নিজের স্বপ্নগুলোকে
        কখনো ছেড়ে দিও না।
      </p>

      <p>
        আবারও তোমাকে জানাই
        <strong>শুভ জন্মদিন। 🎂🎉</strong>
      </p>

      <div class="signature">
        অনেক ভালোবাসা ❤️<br>
        তোমার আপনজন
      </div>

    </div>

  </section>

  <div class="footer">
    Made with ❤️ just for you
  </div>

</div>


<script>
/* Lightweight falling petals */
const symbols = ["🌸","🌷","💮","🌺","✿"];

function createPetal(){

  const petal = document.createElement("div");

  petal.className = "petal";
  petal.textContent =
    symbols[Math.floor(Math.random()*symbols.length)];

  petal.style.left =
    Math.random()*100 + "vw";

  petal.style.fontSize =
    (12 + Math.random()*12) + "px";

  petal.style.animationDuration =
    (5 + Math.random()*5) + "s";

  petal.style.animationDelay =
    Math.random()*2 + "s";

  document.body.appendChild(petal);

  setTim
  },10000);
}

/* Only a few petals at a time = smooth on mobile */
setInterval(createPetal,700);
</script>

</body>
</html>
```
 
