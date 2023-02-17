---
layout: post
title: "&nbsp;"

---
![alt text](https://jonkalev.s3.us-west-2.amazonaws.com/20230216_Neal-Lewis.jpg)
<p style="color: grey; font-size: 16px;">The  <a href="https://www.lensculture.com">Lens Culture</a> portrait entry from earlier today</p>

<body>

<div class="slideshow-container">
  <div class="mySlides fade">
    <img src="https://jonkalev.s3.us-west-2.amazonaws.com/20230215_David+Bramirez.jpg" style="width:100%">
    <div class="text"></div>
  </div>

  <div class="mySlides fade">
    <img src="https://jonkalev.s3.us-west-2.amazonaws.com/20230216_Kenny-Glasgow.jpg" style="width:100%">
    <div class="text"></div>
  </div>

  <div class="mySlides fade">
    <img src="https://jonkalev.s3.us-west-2.amazonaws.com/20230216_Tracy-Barron.jpg" style="width:100%">
    <div class="text"></div>
  </div>

  <div class="mySlides fade">
    <img src="https://jonkalev.s3.us-west-2.amazonaws.com/20230216_Neal-Lewis.jpg" style="width:100%">
    <div class="text"></div>
  </div>

  <div class="mySlides fade">
    <img src="https://jonkalev.s3.us-west-2.amazonaws.com/20230216_three-cousins.jpg" style="width:100%">
    <div class="text"></div>
  </div>

  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
  <span class="dot" onclick="currentSlide(4)"></span> 
  <span class="dot" onclick="currentSlide(5)"></span> 
</div>


  <style>
    .slideshow-container {
      max-width: 1000px;
      position: relative;
      margin: auto;
    }


    .mySlides {
        display: none;
    }
    
    .prev, .next {
      cursor: pointer;
      position: absolute;
      top: 50%;
      width: auto;
      margin-top: -22px;
      padding: 16px;
      color: white;
      font-weight: bold;
      font-size: 18px;
      transition: 0.6s ease;
      border-radius: 0 3px 3px 0;
    }
    
    .next {
      right: 0;
      border-radius: 3px 0 0 3px;
    }
  </style>


  <script>
    var slideIndex = 1;
    showSlides(slideIndex);

    function plusSlides(n) {
      showSlides(slideIndex += n);
    }
    
    function currentSlide(n) {
      showSlides(slideIndex = n);
    }
    
    function showSlides(n) {
      var i;
      var slides = document.getElementsByClassName("mySlides");
      var dots = document.getElementsByClassName("dot");
      if (n > slides.length) {slideIndex = 1}
      if (n < 1) {slideIndex = slides.length}
      for (i = 0; i < slides.length; i++) {
          slides[i].style.display = "none";
      }
      for (i = 0; i < dots.length; i++) {
          dots[i].className = dots[i].className.replace(" active", "");
      }
      slides[slideIndex-1].style.display = "block";
      dots[slideIndex-1].className += " active";
    }
  </script>

</body>


