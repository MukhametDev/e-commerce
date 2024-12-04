<script setup lang="ts">
import menu from '@/assets/menu.ts'

const menuItems = menu.menu
</script>
<template>
  <header class="flex justify-between items-center">
    <div class="flex gap-[10px]">
      <RouterLink to="/">
        <img src="./../assets/logo.png" alt="logo" />
      </RouterLink>
      <p class="max-w-[148px] text-[12px] font-500 leading-[14px] tracking-[0%] text-light-gray">
        Поставщик продуктов для HoReCa
      </p>
    </div>
    <nav class="text-dark-blue">
      <ul class="flex gap-[16px]">
        <li v-for="item in menuItems">
          <RouterLink :to="item.link">{{ item.name }}</RouterLink>
        </li>
      </ul>
    </nav>
    <div class="flex gap-[10px]">
      <img src="./../assets/icons/tg.png" alt="telegram icon" />
      <img src="./../assets/icons/ws.png" alt="whatsapp icon" />
    </div>
    <div class="text-dark-blue flex flex-col gap-[5px] items-center">
      <a class="text-[18px] leading-[100%] tracking-[0%] font-700" href="tel:+7 (495) 637-82-28"
        >8 (495) 637-82-28</a
      >
      <p class="text-light-gray text-[10px] font-600 leading-[100%] tracking-[.1em]">
        заказать звонок
      </p>
    </div>
  </header>
</template>

<style scoped></style>
