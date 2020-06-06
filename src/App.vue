<template>
  <main>
    <bx-Header />
    <bx-assets-table />
  </main>
</template>

<script>
import BxHeader from '@/components/BxHeader'
import BxAssetsTable from '@/components/BxAssetsTable'

export default {
  name: "App",
  components: {
   BxHeader,
   BxAssetsTable
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
