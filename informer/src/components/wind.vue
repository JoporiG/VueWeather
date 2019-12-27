<template>
<div class="wind">
    <img src="img/wind.png"> {{ wind }} <small>м/с</small>
</div>
</template>

<script>
export default {
  name: 'Wind',
  props: ['wind'],
  data(){
    return {text: ''}
  },
}
</script>