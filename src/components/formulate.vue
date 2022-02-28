<template>
  <div class="form">
    <h2>FORM</h2>
    <!-- some code condensed for display reasons -->
    <FormulateForm
      v-model="values"
      @submit="handleLogin"
    >
      <FormulateInput type="text" name="email" label="Email address" validation="required|email" />
      <FormulateInput type="text" name="password" label="Password" validation="required" />
      <FormulateInput name="terms" type="checkbox" label="I accept, just don't make me read the terms." validation="accepted" />
      <FormulateInput type="submit" label="Login" />
    </FormulateForm>
  </div>
</template>

<script>
export default { data () { return { values: {}, handleLogin: () => alert('Logged in') } } }
</script>

<style scoped>
h2 {
  text-align: center;
  font-size: 18px;
}
.form >>>.formulate-input-error {
  color: red;
}
</style>

