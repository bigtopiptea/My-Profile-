<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <h1 class="text-red-500 uppercase">Test</h1>
      </nav>
    </div>
  </header> -->
  <nav class="bg-black px-2 dark:bg-gray-900">
    <div class="block w-full" id="navbar-default">
      <ul class="flex justify-end p-4 flex-row space-x-2 mt-0 text-sm font-bold">
        <li>
          <RouterLink to="/" class="block py-1.5 px-4 uppercase text-white rounded font-bold hover:text-gray-400 p-0 ">
            Home
          </RouterLink>
        </li>
        <li>
          <RouterLink to="/about"
            class="block py-1.5 px-4 uppercase text-white rounded font-bold hover:text-gray-400 p-0 ">About
          </RouterLink>
        </li>
        <!-- <li>
          <a href="#" class="block  uppercase text-white rounded font-bold hover:text-gray-400 p-0 ">Services</a>
        </li>
        <li>
          <a href="#" class="block uppercase text-white rounded font-bold hover:text-gray-400 p-0 ">Pricing</a>
        </li>
        <li>
          <a href="#" class="block uppercase text-white rounded font-bold hover:text-gray-400 p-0 ">Contact</a>
        </li> -->
      </ul>
    </div>
  </nav>

  <RouterView />
</template>

<style>
.navigation-active-link {
  background-color: white;
  color: black !important;
}
</style>
