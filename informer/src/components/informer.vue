<template>
  <div class="informer-container">
      <temp :temperatureReal="temperatureReal" :temperatureFeel="temperatureFeel"/>
      <div class="flex-break"></div>
      <humidity :humidity="humidity"/>
      <div class="vertical-divider"></div>
      <wind :wind="wind"/>
  </div>
</template>

<script>
import humidity from "/home/joporig/VueWeather/informer/src/components/Humidity.vue"
import temp from "/home/joporig/VueWeather/informer/src/components/temperature.vue"
import wind from "/home/joporig/VueWeather/informer/src/components/wind.vue"
export default{
  name: 'FirstComponent',
  data(){
    return {
      temperatureReal: 1,
      temperatureFeel: '-3.2',
      humidity: 6,
      wind: 20,
    }
  },
  components:{
      humidity, temp, wind
  }
}
</script>

<style scoped>
.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  min-height: 255px;
  padding: 30px;
  background-image: url('/img/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
</style>
