<template>
<div class="temperature">
    <img src="img/thermometer.png">
    <div class="temp-real">{{ temperatureReal }}</div>
    <div class="temp-feel">{{ temperatureFeel }}</div>
</div>
</template>

<script>
export default {
  name: 'temp',
  props: ['temperatureReal', 'temperatureFeel'],
}
</script>