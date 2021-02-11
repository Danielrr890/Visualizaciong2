<!--DOCTYPE html-->
<html lang="en">
<title>Miguel</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body {font-family: "Lato", sans-serif}
.mySlides {display: none}
</style>
<body>

<!-- Navbar -->
<div class="w3-top">
  <div class="w3-bar w3-black w3-card">
    <a class="w3-bar-item w3-button w3-padding-large w3-hide-medium w3-hide-large w3-right" href="javascript:void(0)" onclick="myFunction()" title="Toggle Navigation Menu"><i class="fa fa-bars"></i></a>
    <a href="#" class="w3-bar-item w3-button w3-padding-large">Home</a>
    <a href="#aboutme" class="w3-bar-item w3-button w3-padding-large w3-hide-small">About me</a>
    <a href="#contact" class="w3-bar-item w3-button w3-padding-large w3-hide-small">Contact</a>
    <!--<a href="javascript:void(0)" class="w3-padding-large w3-hover-red w3-hide-small w3-right"><i class="fa fa-search"></i></a>-->
  </div>
</div>

<!-- Navbar on small screens (remove the onclick attribute if you want the navbar to always show on top of the content when clicking on the links) -->
<div id="navDemo" class="w3-bar-block w3-black w3-hide w3-hide-large w3-hide-medium w3-top" style="margin-top:46px">
  <a href="#aboutme" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">About me</a>
  <a href="#contact" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">Contact</a>
</div>

<!-- Page content -->
<div class="w3-content" style="max-width:2000px;margin-top:46px">

  <!-- Automatic Slideshow Images -->
  <div class="mySlides w3-display-container w3-center">
    <img src="https://github.com/MiguelRippe/MiguelRippe.github.io/blob/main/images/brain.jpg?raw=true" style="width:100%" alt="brain">
     <div class="w3-display-bottomleft w3-container w3-text-yellow w3-padding-16 w3-hide-small" style="text-shadow:2px 2px 0 #444">
      <h3>Programming lover</h3>
      <p style="max-width:300px;"><b>"Any fool can write code that a computer can understand. Good programmers write code that humans can understand." – Martin Fowler</b></p>   
    </div>  
  </div>
  <div class="mySlides w3-display-container w3-center">
    <img src="https://github.com/MiguelRippe/MiguelRippe.github.io/blob/main/images/cocuy.jpg?raw=true" style="width:100%" alt="cocuy">
    <div class="w3-display-bottommiddle w3-container w3-text-teal w3-padding-16 w3-hide-small" style="text-shadow:2px 2px 0 #444">
      <h3>Travel lover</h3>
      <p><b> "Jobs fill your pockets, adventures fill your soul."</b></p>    
    </div>
  </div>
  <div class="mySlides w3-display-container w3-center">
    <img src="https://github.com/MiguelRippe/MiguelRippe.github.io/blob/main/images/math.jpg?raw=true" style="width:100%" alt="math">
    <div class="w3-display-bottomright w3-container w3-text-white w3-padding-16 w3-hide-small" style="text-shadow:2px 2px 0 #444">
      <h3>Math lover</h3>
      <p style="max-width:350px;"><b>"There should be no such thing as boring mathematics."— Edsger W. Dijkstra </b></p>    
    </div>
  </div>

  <!-- aboutme Section -->
  <div class="w3-container w3-content w3-center w3-padding-64" style="max-width:800px" id="aboutme">
    <h2 class="w3-wide">Miguel Angel Rippe Espinosa</h2>
    <p class="w3-opacity"><i>Mathematician</i></p>
    <p class="w3-justify"> Hello!!! I'm a mathematician from National University of Colombia, actually I'm finishing my doctoral studies in pure maths (Partial Differential Equations). I have always been passionate about numerical methods and programming. I have worked as a teacher in several universities and 
I love traveling and seeing natural places.</p>
    
  </div>


  <!-- The Contact Section -->
  <div class="w3-container w3-content w3-padding-64" style="max-width:800px" id="contact">
    <h2 class="w3-wide w3-center">CONTACT</h2>
    <p class="w3-opacity w3-center"><i>If you wish, do not hesitate to write</i></p>
    <div class="w3-row w3-padding-32">
      <div class="w3-col m6 w3-large w3-margin-bottom">
        <i class="fa fa-map-marker" style="width:30px"></i> Bogotá, colombia<br>
        <i class="fa fa-envelope" style="width:30px"> </i> Email: mrippee@ucentral.edu.co<br>
      </div>
      
<!-- End Page Content -->
</div>



<!-- Footer -->
<footer class="w3-container w3-padding-64 w3-center w3-opacity w3-light-grey w3-xlarge">
  <a href="https://www.linkedin.com/in/marippee"><i class="fa fa-linkedin w3-hover-opacity"> </i> </a>
  <a href="https://github.com/MiguelRippe"><i class="fa fa-github w3-hover-opacity"> </i> </a>
  <p class="w3-medium">Powered by <a href="https://www.w3schools.com/w3css/default.asp" target="_blank">w3.css</a></p>
</footer>

<script>
// Automatic Slideshow - change image every 4 seconds
var myIndex = 0;
carousel();

function carousel() {
  var i;
  var x = document.getElementsByClassName("mySlides");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  myIndex++;
  if (myIndex > x.length) {myIndex = 1}    
  x[myIndex-1].style.display = "block";  
  setTimeout(carousel, 4000);    
}

// Used to toggle the menu on small screens when clicking on the menu button
function myFunction() {
  var x = document.getElementById("navDemo");
  if (x.className.indexOf("w3-show") == -1) {
    x.className += " w3-show";
  } else { 
    x.className = x.className.replace(" w3-show", "");
  }
}

// When the user clicks anywhere outside of the modal, close it
var modal = document.getElementById('ticketModal');
window.onclick = function(event) {
  if (event.target == modal) {
    modal.style.display = "none";
  }
}
</script>
<!--</body>
</html>-->
