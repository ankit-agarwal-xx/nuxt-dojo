<template>
    <div>
      <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-5 flex justify-between">
          <NuxtLink to="/" class="font-bold">Nuxt Doja</NuxtLink>
          <ul class="flex gap-4">
             <li><NuxtLink to="/">Home</NuxtLink></li>
             <li><NuxtLink to="/about">About</NuxtLink></li>
             <li><NuxtLink to="/product" class="btn">Merch</NuxtLink></li>
          </ul>
        </nav>
      </header>

      <!-- output the page content -->
      <div class="container mx-auto p-5">
          <slot />
      </div>
    </div>
  </template>
  
  <style scoped>
    .router-link-exact-active {
      color: #741192;
    }
  </style>