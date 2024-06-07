<template>
   <img class="user__picture" src="../assets/img/image-boy.jpg" />
   <h1 class="user__name">Iskandar To`lqin</h1>
   <h2 class="user__address">Tashkent, Uzbekistan</h2>
   <p class="user__profession">"Front-end developer and avid reader."</p>
</template>
<script setup></script>
<style>
.user {
   background-color: #000;
}
.user__picture {
   border-radius: 50%;
   margin-bottom: 10px;
}
.user__name {
   font-size: 36px;
   font-weight: 700;
   color: white;
   margin-bottom: 15px;
}
.user__address {
   color: hsl(75, 94%, 57%);
   font-size: 18px;
   font-weight: 500;
   margin-bottom: 20px;
}
.user__profession {
   font-weight: 500;
   font-size: 20px;
   margin-bottom: 18px;
}
@media only screen and (max-width: 768px) {
   .user__picture {
      transform: scale(0.8);
   }
}
@media only screen and (max-width: 540px) {
   .user__picture {
      margin-bottom: 8px;
      transform: scale(0.7);
   }

   .user__name {
      font-size: 30px;
      margin-bottom: 12px;
   }
   .user__address {
      font-size: 16px;
      margin-bottom: 16px;
   }
   .user__profession {
      font-size: 18px;
      margin-bottom: 16px;
   }
}
</style>
