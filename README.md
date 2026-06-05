DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sorry Bby ❤️</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Arial',sans-serif;
}

body{
    background:linear-gradient(135deg,#ff4b5c,#ff8fa3);
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
}

.container{
    background:white;
    width:90%;
    max-width:650px;
    padding:35px;
    border-radius:25px;
    text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.2);
    z-index:2;
}

h1{
    color:#ff4b5c;
    margin-bottom:20px;
}

p{
    color:#444;
    font-size:18px;
    line-height:1.8;
}

button{
    margin-top:25px;
    padding:12px 28px;
    border:none;
    border-radius:30px;
    background:#ff4b5c;
    color:white;
    font-size:18px;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    transform:scale(1.05);
}

#hiddenMessage{
    display:none;
    margin-top:25px;
    color:#ff4b5c;
    font-size:22px;
    font-weight:bold;
}

.heart{
    position:absolute;
    color:white;
    animation:float 6s linear infinite;
    font-size:20px;
}

@keyframes float{
    from{
        transform:translateY(100vh);
        opacity:1;
    }
    to{
        transform:translateY(-100px);
        opacity:0;
    }
}
</style>
</head>
<body>

<div class="container">
    <h1>To My Bby ❤️</h1>

    <p>
        Dear Bby,<br><br>

        I want to say sorry from the bottom of my heart. ❤️<br><br>

        Sometimes my insecurities make me overthink things,
        and because of that I misunderstood situations and hurt you.
        You never deserved that, and I truly regret it. 🥺<br><br>

        Thank you for being patient with me, caring for me,
        and staying by my side. You mean so much to me,
        more than I always know how to express. 🌹<br><br>

        I can't change the mistake I made,
        but I promise to learn from it and become better.
        I never want my fears to make you feel unloved or untrusted. ❤️
    </p>

    <button onclick="showMessage()">
        Click Here ❤️
    </button>

    <div id="hiddenMessage">
        Bby, you are my favorite person. 🌹❤️<br>
        Love, Takla ❤️
    </div>
</div>

<script>
function showMessage(){
    document.getElementById("hiddenMessage").style.display="block";
}

function createHeart(){
    const heart=document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML="❤️";
    heart.style.left=Math.random()*100+"vw";
    heart.style.fontSize=(Math.random()*20+15)+"px";
    document.body.appendChild(heart);

    setTimeout(()=>{
        heart.remove();
    },6000);
}

setInterval(createHeart,300);
</script>

</body>
</html>
