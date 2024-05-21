<style>
h1.hero {
  font-size: 4vw !important; /* Adjusted from a fixed em size to viewport width */
  text-align: center;
  font-weight: 700 !important;
  position: absolute !important;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%); /* Adjust to ensure proper centering */
}

@media (max-width: 768px) {
  h1.hero {
    font-size: 4vw; /* Smaller font size for smaller devices */
  }
}

del,
ins {
  position: relative;
  display: inline-block;
  text-decoration: none;
}

del:after,
ins:after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
}

del:after {
  height: calc(40%);
  border-top: 8px solid red;
  transform: rotateZ(-3deg);
  animation: del 1s ease-in;
}

ins:after {
  height: 100%;
  animation: ins 1s ease-out;
  animation-delay: 1s;
  animation-fill-mode: forwards;
}

@keyframes del {
  0% { width: 0; }
  100% { width: 100%; }
}

@keyframes ins {
  0% { width: 0; background: rgb(255, 255, 0); z-index: -1; }
  100% { width: 100%; background: rgb(255, 255, 0); z-index: -1; }
}
</style>


<div class="container-fluid">
  <h1 class="hero">La Comunidad de gente </br>
    <del>interesada en</del> </br> <ins>que utiliza</ins> </br>Inteligencia Artificial
  </h1>
</div>

<!-- background image -->

![](assets/background.png)