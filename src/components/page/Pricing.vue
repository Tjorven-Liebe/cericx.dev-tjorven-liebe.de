<script setup>
</script>

<template>
  <section class="pricing">
    <h1 id="Features" class="text-uppercase">Pricing</h1>
    <hr />
    <div class="card">
      <h1 class="card-title">
        Fair Payment
      </h1>
      <div class="card-body">
        <p style="padding: 0 15%">I think that time is very valuable as it is a limited resource. Regarding this I don't make static prices as someone on Fiverr would. Instead I am calculating the price of the software after it is done. Don't worry I will not ask for money if there is no finished product in the end. But I will ask if it was recognised as usable from the buyer.</p>
        <hr/>
        <h3 class="text-center">But how do I calculate my prices then?</h3>
        <p style="padding: 0 15%">Obviously hourly. I will track the time I have spent on developing the plugin. I will take the minimum wage of my country <b>13€</b>h.1 <br /> Of course, if the product is not too large, static prices can be considered.</p>
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