<template>
  <div class="panel">
    <div class="header">
      <h2 class="headline">{{ headline }}</h2>
    </div>
    <div class="body">
      content
      <slot/>
    </div>

  </div>

</template>

<script>
  export default {
    name: 'Panel',
    props: {
      headline: String
    }
  }
</script>

<style lang="sass" src="../../assets/styles/Panel.sass"/>
