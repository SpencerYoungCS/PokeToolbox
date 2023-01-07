<script setup>
import EffectiveChart from "./components/EffectiveChart.vue";
import TypeChart from "./components/TypeChart.vue";
</script>

<template>
  <div class="vertical-container">
    <div style="text-align:center">
      <h1>Poketoolbox</h1>
    </div>
    <!-- <a href="https://poketoolbox.net"><img src="@/assets/logo.svg" alt="Logo"></a> -->
    <!-- <h1 style="text-align:center">Title</h1> -->
    <div>
      <EffectiveChart />
    </div>
    <div>
      <TypeChart />
    </div>
  </div>


</template>

<style scoped>
.vertical-container {
  max-width: 1280px;
  display: flex;
  flex-direction: column;
  width: 75vw;
  height: 100%;
}
</style>
