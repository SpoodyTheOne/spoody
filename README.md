
<!doctype html>
<html>
<head>
<title>Plugins, websites and more</title>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
.header {
position: fixed;
top: -8px;
background-color: rgb(255, 50, 50);
text-align: center;
width: 100%;
margin: -8.5px;
font-family: sans-serif;
}

a {
		-moz-transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		-webkit-transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		-ms-transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		
		text-decoration: none;
		color: inherit;
	}

		a:hover {
         color: white;
      }
#test {
font-family: sans-serif;
z-index: 41;
position: fixed;
top: 150px;
display: none;
text-align: center;
background-color: white;

border-radius: 25px;

width: 75%;
position: fixed;
left: 50%;
margin-left: -37.5%;
height: 50%;

overflow: auto
}

#dark {
display: none;
position: fixed;
z-index: 40;
width: 100%;
height: 100%;
margin: -8.3px;
}

#user {
position: relative;
top: 5px;
font-family: sans-serif;
text-align: center;
padding: 0px;
width: 100%;
}

ul, ol {
list-style-type: none;
margin: 0px;
padding: 0px;
}

#password, #name {
width: 80%;
}

#npassword, #renpassword, #nname {
width: 80%;
}

#splitter {
background-color: gray;
width: 100%;
height: 1px;
margin-top: 25px;
}

#about {
font-family: sans-serif;
z-index: 41;
position: fixed;
top: 150px;
display: none;
text-align: center;
background-color: white;

border-radius: 25px;

width: 75%;
position: fixed;
left: 50%;
margin-left: -37.5%;
height: 50%;

overflow: auto
}
</style>
</head>

<body>
<div class="header">
<h2>Spoody</h2>
<p><a href="free.html">Free</a> | <a href="contact.html">Contact me</a> | <a href="buy.html">Buy</a> | <a href="#" id="login">Login</a> | <a href="#" id="bout">About me</a></p>
</div>

<div id="dark">
</div>
<div id="test">
<h3 style="width: 100%; height: 60px; background-color: red; margin-top: -0px; margin-bottom: -50px;">Login</h3>
<p>Or signup</p>
<div id="user">
<ul id="user">
<input type="email" id="name" placeholder="Name / Email">
<br>

<input type="password" id="password" placeholder="Password">
<br>
<button type="submit" id="log">Login</button>
</ul>
<div id="splitter"></div>
<div id="signup">
<ul id="user">
<input type="email" id="nname" placeholder="Name / Email">
<br>

<input type="password" id="npassword" placeholder="Password">
<input type="password" id="renpassword" placeholder="Retype password">
<br>
<button type="submit" id="signup">Signup</button>
</ul>
</div>
</div>
</div>

<div id="about">
<h3 style="width: 100%; height: 60px; background-color: red; margin-top: -0px; margin-bottom: -50px;">About me</h3>
<p><a href="#what">what i make</a> | price | how fast</p>
<div id="what">
<h3>What i make</h3>
<ul id="what">
<p>I make minecraft plugins, websites and more within that catagory. I know JS, HTML and CSS all to a limited extend</p>
</ul>
</div>
</div>
</div>

<script>
var log = document.getElementById("log");

var btn = document.getElementById("login");

var btn2 = document.getElementById("bout");
var bout = document.getElementById("about");

var dark = document.getElementById("dark");

var test =  document.getElementById("test");

var open = false;
var open2 = false

btn.onclick = function() {login()};

dark.onclick = function() {close()};

log.onclick = function() {log()};

btn2.onclick = function() {about()};

function login() {


if (open == false) {
test.style.display = "block";
dark.style.display = "block";

document.getElementById("dark").style.backgroundColor = "#00000050";

open = true;

} else {

test.style.display = "none";
dark.style.display = "none";

document.getElementById("dark").style.backgroundColor = "white";

open = false

}

}

function close() {

test.style.display = "none";
dark.style.display = "none";
bout.style.display = "none";

document.getElementById("dark").style.backgroundColor = "white";

open = false
open2 = false

}

function log() {

var naem = document.getElementById("name").value;

var pass = document.getElementById("password").value;

if (naem == "admin") {
window.location = "http://zochg.ga";

} else {

alert("wrong");

}
}

function about() {


if (open2 == false) {
bout.style.display = "block";
dark.style.display = "block";

document.getElementById("dark").style.backgroundColor = "#00000050";

open2 = true;

} else {

bout.style.display = "none";
dark.style.display = "none";

document.getElementById("dark").style.backgroundColor = "white";

open2 = false

}

}

</script>
</body>
</html>
