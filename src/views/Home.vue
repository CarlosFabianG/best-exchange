<template>
  <div>
    <bounce-loader :loading="isLoading" :color="`#68d391`" :size="100" />
    <bx-assets-table v-if="!isLoading" v-bind:assets="assets" />
  </div>
</template>

<script>
import api from "@/api";
import BxAssetsTable from "@/components/BxAssetsTable";
export default {
  name: "Home",

  components: { BxAssetsTable },

  data() {
    return {
      isLoading: false,
      assets: []
    };
  },
  created() {
    this.isLoading = true
    api.getAssets()
    .then(assets => (this.assets = assets))
    .finally( () => this.isLoading = false)
  }
};
</script>
