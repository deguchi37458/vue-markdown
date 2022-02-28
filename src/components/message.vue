<template>
  <div class="message">
      <h2>MESSAGE BOX</h2>
      <input type="text" v-model="msg">
      <button @click="clear()">clear</button>
      <p v-if="msg.length > 0">
        {{msg}}
      </p>
      <p v-else>
        no text
      </p>
  </div>
</template>
<script>
export default {
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

<style scoped>
.message {
  padding-bottom: 30px;
  margin-bottom: 30px;
  border-bottom: solid 1px #333;
}
h2 {
  text-align: center;
  font-size: 18px;
}
input,
button{
  padding: 5px;
  border: solid 1px#333;
  border-radius: 10px;
}
button:hover{
  cursor: pointer;
}
</style>