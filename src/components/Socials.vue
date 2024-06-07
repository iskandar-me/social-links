<script setup>
import { ref } from "vue";
const socials = ref([
   { name: "Github", url: "https://github.com/Iskandar-me" },
   { name: "LinkedIn", url: "https://linkedin.com/in/iskandar-tolqinov" },
   { name: "X(Twitter)", url: "https://x.com/iskandar_wave" },
   { name: "Instagram", url: "https://instagram.com/iskandar.tolqin" },
   { name: "Telegram", url: "https://t.me/iskandar_wave" },
]);
</script>
<template>
   <ul class="socials__list">
      <li v-for="(social, index) in socials" :key="index">
         <a :href="social.url" class="socials__item" target="_blank">
            {{ social.name }}
         </a>
      </li>
   </ul>
</template>

<style scoped>
.socials__list {
   list-style: none;
   display: flex;
   flex-direction: column;
   gap: 10px;
   color: white;
   font-weight: bold;
   padding: 0;
}
.socials__item {
   display: block;
   background-color: hsl(0, 0%, 12%);
   text-decoration: none;
   color: white;
   padding: 12px 8px;
   border-radius: 10px;
   cursor: pointer;
   font-size: 14px;
   transition: all 0.4s ease;
}
.socials__item:hover {
   background-color: hsl(75, 94%, 57%);
   color: hsl(0, 0%, 10%);
   font-weight: bold;
}
@media only screen and (max-width: 540px) {
   .socials__item {
      font-size: 12px;
      padding: 10px 6px;
   }
}
</style>
