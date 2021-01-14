<template>
  <div>
    <p>bonjour</p>
    <h1 class="fond" id="yoo">alloooooooooooooo</h1>
  </div>
  <span>{{ allo }}</span>
  <span>{{ compteur }}</span>
</template>

<style scoped>
/* scoped c pour ces css n'affeter pas les autres scripts. ONLY les divs dans ce script*/
  div {
    background-color: white;
  }
  #yoo {
    color: blue;
  }
  
  .fond {
    background-color: lightgreen;
    color: aqua;
  }
</style>

<script>
export default {
  data() {
    return {
      allo : 'bonjour',
      compteur: 0,
    }
  }
}
</script>