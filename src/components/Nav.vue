<script setup>
import NavLink from "./NavLink.vue";
import { RouterLink } from "vue-router";
</script>

<template>
  <nav class="bg-gray-800 p-4">
    <div class="container mx-auto flex justify-between items-center">
      <RouterLink class="text-white text-xl font-bold" to="/">Mon site</RouterLink>

      <div class="space-x-4">
        <ul class="flex">
          <NavLink url="/" text="Accueil" class="text-white hover:text-blue-300" />
          <span class="mx-2"></span> <!-- Espace entre les liens -->
          <NavLink url="/chat" text="Chat" class="text-white hover:text-blue-300" />
        </ul>
      </div>
    </div>
  </nav>
</template>