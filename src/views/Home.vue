<template>
<div>
 <!-- ======= Hero Section ======= -->
  <section id="hero">
    <div class="hero-container">
      <h1>Chalinas Design_</h1>
      <h2>Ruanas & más | Productos 100% chilenos</h2>
      
      <a href="#about" class="btn-scroll scrollto" title="Scroll Down"><i class="bx bx-chevron-down"></i></a>
    </div>
  </section><!-- End Hero -->
<productos/>
</div>

</template>

<script>




export default {
  name: 'Home',
  components:{

  }
}
</script>

<style lang="scss">

//home { 
  //background-image: url('../assets/img/fondoamarillo.jpg');
  //background-size: cover;
  //background-repeat: no-repeat;
  //background-position: center top;
  //height: 100vh;


#hero {
  width: 100%;
  height: 100vh;
  background: url("../assets/img/fondoamarillo.jpg") top right;
  background-size: cover;
  position: relative;
}

#hero:before {
  content: "";
  background: rgba(0, 0, 0, 0.65);
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
}

#hero .hero-container {
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 0 15px;
}

#hero h1 {
  margin: 0 0 10px 0;
  font-size: 64px;
  font-family: "Satisfy", serif;
  color: #fff;
}

#hero h2 {
  color: #eee;
  margin-bottom: 50px;
  font-size: 13px;
  font-weight: 500;
  letter-spacing: 1px;
  text-transform: uppercase;
}

#hero .btn-scroll {
  transition: 0.4s;
  color: rgba(255, 255, 255, 0.6);
  animation: up-down 1s ease-in-out infinite alternate-reverse both;
}

#hero .btn-scroll i {
  font-size: 48px;
}

#hero .btn-scroll:hover {
  color: #ffb727;
}

@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}

@media (max-width: 575px) {
  #hero h1 {
    font-size: 40px;
  }
  #hero h2 {
    text-align: center;
    margin-bottom: 30px;
  }
}

@-webkit-keyframes up-down {
  0% {
    transform: translateY(5px);
  }
  100% {
    transform: translateY(-5px);
  }
}

@keyframes up-down {
  0% {
    transform: translateY(5px);
  }
  100% {
    transform: translateY(-5px);
  }
}




</style>