<template>
  <Mifos v-if="product == 'mifos'" />
  <PpinaBox v-else-if="product == 'ppinabox'" />
  <SearchApp v-else-if="product == 'search-app'" />
</template>

<script setup lang="ts">
import { onMounted, computed } from "vue";
import { useRoute } from "vue-router";
import Mifos from "@/components/products/Mifos.vue";
import PpinaBox from "@/components/products/PpinaBox.vue";
import SearchApp from "@/components/products/SearchApp.vue";

const route = useRoute();

const product = computed(() => {
  return route.params.product;
});

onMounted(() => {
  // if (!route.params.product) return router.push("/");
});
</script>
