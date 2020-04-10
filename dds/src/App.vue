
<template>

  <div id="app">   
    
    <div class="logo-container"> 
      <img src="@/assets/dds-logo.svg" class="logo" />
    </div>

    <Home msg="dds" class="hidden" />

  </div>

</template>

<script>

import Home from '@/components/Home'

export default {

  name: 'App',

  data () {
    return {
      test: 'beep'
    }    
  },

  components: {
    Home
  }
}

</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=Barlow&display=swap');

$bgC: 'background-color';
$dark: #232323;
$dark-light: #282828;
$brown: #444040;
$dorange: #FF6101;
$grey: #f8f8f8;
$white: #ffffff;

body {
  background-color: $dark;
  font-family: 'Barlow', sans-serif;
  color: $white;
}

.logo {
  width: 74px;
  height: 74px;
}

.logo-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 95vh;  
}

.hidden {
  display: none;
}

</style>
