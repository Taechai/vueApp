<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import IconLogo from './components/icons/IconLogo.vue'
import IconMail from './components/icons/IconMail.vue'
import IconNotification from './components/icons/IconNotification.vue'
import IconProfile from './components/icons/IconProfile.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <IconLogo />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/dashboard">Dashboard</RouterLink>
        <RouterLink to="/processes">Processes</RouterLink>
        <RouterLink to="/messages">
          <IconMail />
        </RouterLink>
        <RouterLink to="/notifications">
          <IconNotification />
        </RouterLink>
        <RouterLink to="/profile">
          <IconProfile />
        </RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style>

</style>
