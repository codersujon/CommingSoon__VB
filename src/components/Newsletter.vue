<script setup>

</script>

<template>
    <div class="bg0 wsize1 bor1 p-l-45 p-r-45 p-t-50 p-b-18 p-lr-15-sm">
        <h3 class="l1-txt3 txt-center p-b-43">
          Newsletter
        </h3>

        <form class="w-full validate-form">

          <div class="wrap-input100 validate-input m-b-10" data-validate = "Name is required">
            <input class="input100 placeholder0 s1-txt1" type="text" name="name" placeholder="Name">
            <span class="focus-input100"></span>
          </div>

          <div class="wrap-input100 validate-input m-b-20" data-validate = "Valid email is required: ex@abc.xyz">
            <input class="input100 placeholder0 s1-txt1" type="text" name="email" placeholder="Email">
            <span class="focus-input100"></span>
          </div>

          <button class="flex-c-m size2 s1-txt2 how-btn1 trans-04">
            Subscribe
          </button>
        </form>

        <p class="s1-txt3 txt-center p-l-15 p-r-15 p-t-25">
          And don’t worry, we hate spam too! You can unsubcribe at anytime.
        </p>
      </div>
</template>