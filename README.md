<!DOCTYPE html>
<html>
<head>
  .cursor {
  display: inline-block;
  background-color: #00ffcc;
  width: 10px;
  animation: blink 0.7s steps(1) infinite;
  margin-left: 3px;
}

@keyframes blink {
  50% { background-color: transparent; }
}

.typed-text {
  color: #00ffcc;
  font-family: 'Courier New', monospace;
  font-size: 32px;
}

  <title>Adithyan | Cybersecurity Portfolio</title>
</head>
<body>
 
  <h1><span class="typed-text"></span><span class="cursor">|</span></h1>
  <p>Ethical Hacker | Network Sleuth | Bug Hunter in Training</p>
  <script>
const text = "init Adithyan_H | Cybersecurity_Activated 🛡️";
let index = 0;
const typedText = document.querySelector(".typed-text");

function type() {
  if (index < text.length) {
    typedText.textContent += text.charAt(index);
    index++;
    setTimeout(type, 80);
  }
}

window.onload = type;
</script>

</body>
</html>
