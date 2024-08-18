<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container p-4 flex justify-between items-center">
        <NuxtLink class="font-bold" to="/">JUJUTSU LOGO</NuxtLink>
        <ul class="flex gap-4">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products" class="btn">products</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <!-- output the page content -->
    <div class="container mx-auto">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.router-link-active {
  color: rgb(46, 149, 2);
}
</style>
