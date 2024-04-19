<script setup>

import Animation from '@/components/Animation.vue'
import { Typed } from '@duskmoon/vue3-typed-js'
import { ref } from 'vue'

const links = ref({
  github: {
    link: 'https://github.com',
    icon: 'fa-github',
    color: '#24292e'
  },
  discord: {
    link: 'https://discord.com/users/428284027519369217',
    icon: 'fa-discord',
    color: '#7289da'
  }
})

let props = defineProps(['imageSource'])

const options = {
  strings: ['I am <b>Tjorven Liebe</b>!',
    'Nice to meet you!',
    'This is my website.',
    'Feel free to look around a bit!',
    'If you have <b>questions</b>..',
    '..don\'t hesitate to ask them on <b><a href=\'https://discord.com/users/428284027519369217\'>Discord</a></b>.',
    'Also have a look at my <b><a href=\'https://github.com/Tjorven-Liebe\'>GitHub</a></b>',
    'Well then.. Enjoy looking around and I wish you an awesome day!'],
  loop: true,
  typeSpeed: 20,
  fadeOut: 20,
  showCursor: false
}
</script>

<template>
  <section class="bg">
    <Animation />
    <div class="padding"></div>
    <div class="box-bottom"></div>
    <div class="container">
      <div class="row">
        <div class="col-sm-6 col-12">
          <div class="box">
            <h1>Hello there!</h1>
            <Typed :options="options" class="type-container">
              <h1 class="typing"></h1>
            </Typed>
            <div class="contact">
              <ul class="brands">
                <li class="brand-icons" v-for="item in links">
                  <a :style="'color: ' + item.color" :href="item.link">
                    <i :class="'fab ' + item.icon + ' fa-3x'"></i>
                  </a>
                </li>
              </ul>
              <h6 class="text-center text-uppercase fw-bolder">Contact me</h6>
            </div>
            <span id="title"></span>
          </div>
        </div>
        <div class="col-5 offset-lg-1">
          <div class="mt-5 mt-lg-0">
            <img :src="props.imageSource" alt="" class="image mx-auto d-block" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>

.contact {
  margin-top: 2%;
  margin-bottom: 12%;
  border-bottom: 2px solid var(--color-text);
  padding-bottom: 10px;
  border-radius: 5px;

  .brands {
    transform: translateX(-6px);
    display: flex;
    justify-content: center;
    list-style-type: none;
    li {
      display: inline;
    }
    .brand-icons {
      :not(:hover) {
        color: var(--color-text) !important;
        transition: color 1s !important;
      }
      margin-right: 15px;
      text-decoration: none;
    }
  }
}



.type-container {
  height: 180px;
}

.bg {
  position: relative;
  display: block;

  .box-bottom {
    background: #181926;
    width: 150%;
    height: 35%;
    rotate: -3deg;
    z-index: -1;
    position: absolute;
    bottom: -13%;
    left: -30%;
    box-shadow: 0 0 3px 6px #181926;
  }
}

@media only screen and (max-width: 830px) {
  .image {
    display: none !important;
  }
  .bg .box-bottom {
    display: none;
  }
}

.image {
  margin-top: 20vh;
  height: 400px;
}

.padding {
  padding-top: 20vh;
}
</style>