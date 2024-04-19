<script setup>
</script>

<template>
  <section class="pricing">
    <h1 id="Features" class="text-uppercase">Features</h1>
    <hr />
    <div class="container">
      <div class="row">
        <div class="col-lg">
          <div class="card h-100">
            <h1 class="card-title">Highly Customizable</h1>
            <div class="card-body" style="text-align: start">
              Making the produced software customizable is the bare minimum a professional programm should have.<br/>
              By making my software easy to customize and configure I ensure a professional quality and best user experience.
              <br/><br />
            </div>
          </div>
        </div>
        <div class="col-lg">
          <div class="card h-100">
            <h1 class="card-title">Development</h1>
            <div class="card-body" style="text-align: start">
              Minecraft is full of possibilities, you just have to use them!<br />
              I am tailoring specialized software that is able to enable thousands of possibilities regarding minecraft
              servers.<br />
              <hr />
              <h1 class="justify">(Code-) Quality</h1>
              <div class="d-flex" style="text-align: start">I ensure the best performance by using the most powerful software. Also I am doing my best
                to create the best possible software <a href="https://papermc.io/"><img
                  alt height="128" src="https://tjorven-liebe.de/assets/paper.png" style="margin-left: 15px" /></a>
              </div>
              <hr />
            </div>
          </div>
        </div>
        <div class="col-lg">
          <div class="card h-100">
            <h1 class="card-title">Fast Support!</h1>
            <div class="card-body" style="text-align: start">
              Who ever has bought software knows that the support of software is very important. Not only security updates but bug fixes on request are part of my service.<br/>
              As mentioned above you can easily contact me on Discord. If wished other communication solutions are thinkable. But reaction time will be limited.
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="box-bottom"></div>
  </section>
</template>

<style lang="scss" scoped>
.pricing {
  position: relative;
  margin-bottom: 15%;
  .card {
    background: #181926;
  }

  padding: 7% 5% 2%;

  * {
    text-align: justify;
  }

  h1 {
    text-align: center;
  }

  .box-bottom {
    background: #181926;
    width: 150%;
    height: 35%;
    rotate: 1deg;
    z-index: -1;
    position: absolute;
    bottom: -50%;
    left: -30%;
    box-shadow: 0 0 3px 6px #181926;
  }
}

@media only screen and (max-width: 830px) {
  .bg .box-bottom {
    display: none;
  }
}


</style>