<template>
  <div id="schedule">
    <Calendar/>  
  </div>
</template>

<script>

import Calendar from "../components/Calendar.vue"


export default {
  name: 'Schedule',
  data: function(){
    return {
      partidos: [],
    }
  },
  components: {
    Calendar,
  },
}
</script>

<style>
  #schedule{
  max-height: 5vh;
  }
</style>