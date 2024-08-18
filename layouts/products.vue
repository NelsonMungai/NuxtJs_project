<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4">
        <NuxtLink class="font-bold" to="/products"
          >JUJUTSU LOGO PRODUCTS</NuxtLink
        >
      </nav>
    </header>
    <!-- output the page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
    <footer
      class="container border-t-2 border-gray-300 p-4 flex justify-between mx-autoss"
    >
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/products">products</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
NuxtLink {
  color: yellow;
}
.router-link-active {
  color: aqua;
}
</style>
