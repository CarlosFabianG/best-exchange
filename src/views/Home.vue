<template>
  <div>
    <bx-assets-table v-bind:assets="assets"/>
  </div>
</template>

<script>
import api from "@/api"
import BxAssetsTable from "@/components/BxAssetsTable";
export default {
  name: "Home",

  components: { BxAssetsTable },

  data(){
      return {
          assets: []
      }
  },
  created(){
      api.getAssets()
      .then(assets => (this.assets = assets))
  }
};
</script>
