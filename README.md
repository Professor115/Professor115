
<html>
<style>
*{
	margin:0px;
	padding:0px;
}
#body{
	background:black;
}
#search{
	width:80%;
	height:100px;
	margin-top:150px;
	background:#282828;
	border-radius:25px;
	font-size:45px;
	color:white;
	border:none;
	transition:0.4s;
}
#search:focus{
	border:none;
	outline:none;
	width:75%;
	margin-right:70px;
}
#filter{
	width:100px;
	height:75px;
	background:transparent;
	color:#0CAFFF;
	font-size:40px;
	border:none;
	margin-left:20px;
	visibility:visible;
}
#runf{
	width:100%;
	height:700px;
	background:#272727;
	border:none;
	border-radius:45px;
	margin-top:1400px;
	position:fixed;
	visibility:hidden;
	transition:0.5s;
	z-index:1;
}
#cens{
	width:100%;
	height:100%;
	background:black;
	z-index:0;
	position:fixed;
	visibility:hidden;
	opacity:0%;
	transition:0.5s;
}
#cens2{
	width:100%;
	height:100%;
	background:black;
	z-index:1;
	position:fixed;
	visibility:hidden;
	opacity:0%;
	transition:0.5s;
}
.tas{
	width:320px;
	height:130px;
	background-color:transparent;
	border:none;
	border-bottom:none;
	font-size:40px;
	margin-left:0px;
	color:darkgray;
	transition:0s;
	transition-delay:0s;
}
.tas:hover{
	color:white;
	border-bottom:3px solid white;
}
#ui{
	margin-top:3px;
}
.chat{
	width:100%;
	height:180px;
	background:transparent;
	transition:0.2s;
}
.chat:hover{
	background:#272727;
}
.img{
	width:155px;
	height:155px;
	background-image:url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTXavYob1AQSCP71cr-RZUP6b_i7uYwSKwzPw&usqp=CAU");
	border-radius:100px;
	background-position: center;
	margin:30px;
	margin-top:50px;
}
.user{
	color:white;
	margin-left:200px;
	margin-top:-160px;
	font-size:38px;
	font-family:sans-serif;
}
.seen{
	color:gray;
	margin-left:215px;
	margin-top:10px;
	font-size:38px;
	font-family:sans-serif;
}
.svg{
	width:70px;
	height:70px;
	color:gray;
	margin-left:890px;
	align-items:center;
	margin-top:-65px;
}
#p{
	visibility:visible;
	transition:0s;
}
#canc{
	margin-left:-185px;
	width:150px;
	height:70px;
	background:transparent;
	color:#ffffff;
	font-size:45px;
	border:none;
	z-index:2;
	visibility:hidden;
	transition:0s;
}
</style>
<body id="body">
<div id="cens" onclick="pro()"></div>
<div id="cens2" onclick="pro2()"></div>
<center><input type="search" id="search" onclick="sear()" placeholder="Search">
<button id="filter" onclick="filter()"><p id="p">Filter</p></button>
<button id="canc" onclick="hidd();">Cancel</button>
<div id="runf"></div>
</center>
<button class="tas" id="pri">Primary</button>
<button class="tas" id="gen">General</button>
<button class="tas" id="req">Requests</button>
<ul id="ui">
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">0.715</p>
<p class="seen">Seen 3h ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">aayth</p>
<p class="seen">Seen 12m ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">3.9.9.6</p>
<p class="seen">Seen 1day ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">_tkt0_</p>
<p class="seen">Seen yesterday</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">Username</p>
<p class="seen">Seen 1Y ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">x8.y2</p>
<p class="seen">Seen 7h ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">o1.1i1</p>
<p class="seen">Seen 3w ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">Lil nas X</p>
<p class="seen">Seen 2 ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></li>
<li><a href="#"><div class="chat" onclick="backdiv()">
<div class="img"></div>
<p class="user">Opiilz</p>
<p class="seen">Seen 2y ago</p>
<svg class="svg" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-camera" viewBox="0 0 16 16">
  <path d="M15 12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h1.172a3 3 0 0 0 2.12-.879l.83-.828A1 1 0 0 1 6.827 3h2.344a1 1 0 0 1 .707.293l.828.828A3 3 0 0 0 12.828 5H14a1 1 0 0 1 1 1v6zM2 4a2 2 0 0 0-2 2v6a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2h-1.172a2 2 0 0 1-1.414-.586l-.828-.828A2 2 0 0 0 9.172 2H6.828a2 2 0 0 0-1.414.586l-.828.828A2 2 0 0 1 3.172 4H2z"/>
  <path d="M8 11a2.5 2.5 0 1 1 0-5 2.5 2.5 0 0 1 0 5zm0 1a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7zM3 6.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0z"/>
</svg>
</div></a></li>
</ul>
<script>
function pro(){
	window.cens.style.opacity="0%";
	window.runf.style.marginTop="1450px";
	window.cens.style.visibility="hidden";
window.runf.style.visibility="hidden";
}
function filter(){
window.runf.style.visibility="visible";
	window.runf.style.marginTop="790px";
	window.cens.style.opacity="70%";
	window.cens.style.visibility="visible";
	
}
function backdiv(){
	window.chat.style.background="#272727"
}



function sear(){
window.p.style.visibility="hidden";
	window.canc.style.visibility="visible";
		window.cens2.style.visibility="visible";
}
function pro2(){
	document.getElementById("search").blur()
	window.canc.style.visibility="hidden";
	window.p.style.visibility="visible";

window.cens2.style.visibility="hidden"
}
function hidd(){
	document.getElementById("search").blur()
	window.canc.style.visibility="hidden";
	window.p.style.visibility="visible";


}
</script>
</body>
</html>
