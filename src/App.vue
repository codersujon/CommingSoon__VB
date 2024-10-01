<script setup>
import Logo from '@/components/Logo.vue'
import SocialMediaIcon from './components/SocialMediaIcon.vue';
import Newsletter from './components/Newsletter.vue';
const ourws = "Our website is"
const cs = "Coming Soon"
</script>

<template>
  <div class="bg-img1 size1 overlay1 p-t-24" style="background-image: url('/src/assets/images/bg01.jpg');">
    <div class="flex-w flex-sb-m p-l-80 p-r-74 p-b-175 respon5">
      
      <!-- logo -->
      <Logo />

      <!-- Social Icon -->
      <SocialMediaIcon />

    </div>

    <div class="flex-w flex-sa p-r-200 respon1">
      <div class="p-t-34 p-b-60 respon3">
        <p class="l1-txt1 p-b-10 respon2">{{ ourws }}</p>
        <h3 class="l1-txt2 p-b-45 respon2 respon4">{{ cs }}</h3>
        <div class="cd100"></div>
      </div>

      <!-- Newsletter -->
      <Newsletter />
    </div>
  </div>
</template>


