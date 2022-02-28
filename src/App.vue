<template>
  <div class="wrapper">
    <myheader></myheader>
    <message></message>
    <formulate></formulate>
    <myfooter></myfooter>
  </div>
</template>

<script>
import myheader from './components/myheader'
import myfooter from './components/myfooter'
import message from './components/message'
import formulate from './components/formulate'

export default {
  components: {
    myheader,
    myfooter,
    message,
    formulate
  },
}
</script>

<style scoped>
.wrapper {
  width: 1000px;
  margin: 0 auto;
}
</style>