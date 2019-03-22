<template>
  <div id="app">
    <Panel class="groundsman-panel" headline="Test123">
    </Panel>
    <main>
      <LoginForm></LoginForm>

    </main>
  </div>
</template>

<script>
import Panel from './components/core/Panel.vue'
import LoginForm from './components/core/LoginForm'
export default {
  name: 'app',
  components: {
    LoginForm,
    Panel
  }
}
</script>

<style lang="sass">
body
  margin: 0


#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  color: #2c3e50


main
  text-align: center
  margin-top: 40px


header
  margin: 0
  height: 56px
  padding: 0 16px 0 24px
  background-color: #35495E
  color: #ffffff

  span
    display: block
    position: relative
    font-size: 20px
    line-height: 1
    letter-spacing: .02em
    font-weight: 400
    box-sizing: border-box
    padding-top: 16px
</style>
