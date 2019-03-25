<template>
  <form>
    <Input
      type="input"
      label="Username"
      v-model="inputs.username"
      @input="input"/>
    <Input
      type="input"
      label="Passwort"
      v-model="inputs.password"
      @input="input"/>
  </form>
</template>

<script>
  import Input from './Input'
  export default {
    name: 'LoginForm',
    components: {
      Input
    },
    data () {
      return {
        inputs: {
          username: '',
          password: ''
        }
      }
    },
    methods: {
      input: function (input) {
        if (input.type !== 'input') {
          this.username = ''
          this.password = ''
        }
      }
    }
  }
</script>

<style lang="sass" src="../../assets/styles/LoginForm.sass"/>
