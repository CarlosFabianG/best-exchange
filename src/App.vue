<template>
  <main>
    <bx-Header/>
  </main>
</template>

<script>
import BxHeader from '@/components/BxHeader'

export default {
  name: "App",
  components: {
   BxHeader
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
