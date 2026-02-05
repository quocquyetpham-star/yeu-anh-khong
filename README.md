<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Yêu anh không? 😳</title>

<style>
body{
background:linear-gradient(135deg,#ff9a9e,#fad0c4);
margin:0;
font-family:Arial;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
}
.box{
background:white;
padding:30px;
border-radius:15px;
text-align:center;
box-shadow:0 0 20px rgba(0,0,0,0.2);
}
h1{color:#ff4d6d;}
button{
padding:12px 20px;
font-size:16px;
border:none;
border-radius:8px;
cursor:pointer;
margin:10px;
}
#yesBtn{background:#ff4d6d;color:white;}
#noBtn{background:#333;color:white;}
</style>
</head>

<body>

<div class="box" id="box">
<h1>Yêu anh không? 😳</h1>
<button id="yesBtn">CÓ ❤️</button>
<button id="noBtn">KHÔNG 😅</button>
</div>

<script>
const noBtn=document.getElementById("noBtn");
const yesBtn=document.getElementById("yesBtn");

function move(){
const x=Math.random()*(window.innerWidth-100);
const y=Math.random()*(window.innerHeight-50);
noBtn.style.position="fixed";
noBtn.style.left=x+"px";
noBtn.style.top=y+"px";
}
noBtn.addEventListener("mouseenter",move);
noBtn.addEventListener("click",move);

yesBtn.onclick=function(){
document.getElementById("box").innerHTML=
"<h1>Anh biết mà 😎💖</h1><h2>LOVE YOU ❤️</h2>";
};
</script>

</body>
</html>
