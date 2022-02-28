<template>
  <div>
    <myheader></myheader>
    <p v-if="msg.length > 0">
      {{msg}}
    </p>
    <p v-else>
      no text
    </p>
    <input type="text" v-model="msg">
    <button @click="clear()">clear</button>
    <myfooter></myfooter>
    <formulate></formulate>
  </div>
</template>

<script>
import myheader from './components/myheader'
import myfooter from './components/myfooter'
import formulate from './components/formulate'

export default {
  components: {
    myheader,
    myfooter,
    formulate
  },
  data () {
    return {
      msg: 'Hello World!'
    }
  },
  methods: {
    clear () {
      this.msg = ''
    }
  }
}
</script>

