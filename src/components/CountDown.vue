<script setup>
  import {ref, onMounted} from "vue";
  // Project EndDate
  const EndDate = new Date("Oct 15, 2024").getTime();

  const d = ref("");
  const h = ref("");
  const m = ref("");
  const s = ref("");

  // Handle Project End Date
  const handleProjectDate = () =>{
      let now = new Date().getTime();
      let gap = EndDate - now;

      let second = 1000;
      let minute = second * 60;
      let hour = minute * 60;
      let day = hour * 24;

      d.value = Math.floor(gap / (day));
      h.value = Math.floor(gap % (day) / (hour));
      m.value = Math.floor(gap % (hour) / (minute));
      s.value = Math.floor(gap % (minute) / (second));
  }

  // onMounted
  onMounted(()=>{
      setInterval(()=>{
        handleProjectDate();
      },1000); // Every 1000 milisecond
  });


</script>

<template>
  <div class="countdown d-flex">
    <div class="time mx-2 text-center">
      <h2 class="d">{{ d }}</h2>
      <span>Days</span>
    </div>
    <div class="time mx-2 text-center">
      <h2 class="h">{{ h }}</h2>
      <span>Hours</span>
    </div>
    <div class="time mx-2 text-center">
      <h2 class="m">{{m}}</h2>
      <span>Minutes</span>
    </div>
    <div class="time mx-2 text-center">
      <h2 class="s">{{s}}</h2>
      <span>Seconds</span>
    </div>
  </div>
</template>

<style scoped>

.time {
  width: 120px;
  background: #0d1629;
  padding: 20px;
  line-height: -10;
  border-radius: 10px;
  color: #fff;
}

.time h2{
  font-size: 60px;
  font-weight: bold;
}

.time span {
  font-size: 20px;
}

</style>