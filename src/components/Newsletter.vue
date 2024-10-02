<script setup>

  import PrimaryBtn from './PrimaryBtn.vue';
  import InputField from './InputField.vue';

  const title = "Newsletter";
  const content = "And don’t worry, we hate spam too! You can unsubcribe at anytime."

</script>

<template>
    <div class="bg0 wsize1 bor1 p-l-45 p-r-45 p-t-50 p-b-18 p-lr-15-sm">
        <h3 class="l1-txt3 txt-center p-b-43">{{ title }}</h3>

        <form class="w-full validate-form">
          <InputField placeholder="Name" label="name" dataValidate="Name is required "/>
          <InputField placeholder="Email" type="email" label="email" dataValidate="Valid email is required: ex@abc.xyz"/>
          <PrimaryBtn title="Subscribe" />
        </form>

        <p class="s1-txt3 txt-center p-l-15 p-r-15 p-t-25">{{ content }}</p>
      </div>
</template>