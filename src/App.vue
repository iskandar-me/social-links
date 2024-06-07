<script setup>
import Data from "./components/Data.vue";
import Socials from "./components/Socials.vue";
</script>

<template>
   <div class="user">
      <Data></Data>
      <Socials></Socials>
   </div>
</template>

<style scoped>
.user {
   border-radius: 12px;
   background-color: hsl(0, 0%, 8%);
   padding: 30px 24px;
}
</style>
