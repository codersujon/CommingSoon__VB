<script setup>
    defineProps({
        label: String,
        placeholder:{
            type: String,
            default: ""
        },
        type:{
            type: String,
            default: "text"
        },
        dataValidate: String,
    });
</script>
<template>
    <div class="wrap-input100 validate-input m-b-10" :data-validate = "dataValidate">
        <input class="input100 placeholder0 s1-txt1" 
        :type="type" 
        :name="label" 
        :placeholder="placeholder">
        <span class="focus-input100"></span>
    </div>
</template>
