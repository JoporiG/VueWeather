<template>
    <div class="humidity">
        <img src="img/humidity.png"> {{ humidity }} <small>%</small>
    </div>
</template>

<script>
export default {
  name: 'Hum',
  props: ['humidity'],
  data(){
    return {text: ''}
  },
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