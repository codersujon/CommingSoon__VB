<script setup>
defineProps({
    link: String,
    icon: String,
})
</script>
<template>
     <a :href="link" class="size3 flex-c-m how-social trans-04 m-r-6" target="_blank">
          <i :class="`fa fa-${icon}`"></i>
     </a>
</template>
