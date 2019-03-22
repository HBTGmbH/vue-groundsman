<template>
  <form>
    <Input
      type="input"
      label="Username"
      v-model="inputs.username"
      @input="input"/>
  </form>
</template>

<script>
  import Input from './Input'
  export default {
    name: 'LoginForm',
    components: {
      Input
    }
  }
</script>

<style lang="sass" src="../../assets/styles/LoginForm.sass"/>
