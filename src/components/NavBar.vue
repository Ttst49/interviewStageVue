<script setup>
import {
  FwbNavbar,
  FwbNavbarCollapse,
  FwbNavbarLink,
  FwbNavbarLogo,
} from "flowbite-vue";
</script>

<template>
  <fwb-navbar>
    <template #logo>
      <fwb-navbar-logo
        alt="Flowbite logo"
        image-url="../assets/images/logo.png"
        link="/"
      >
        Flowbite
      </fwb-navbar-logo>
    </template>
    <template #default="{ isShowMenu }">
      <fwb-navbar-collapse :is-show-menu="isShowMenu">
        <fwb-navbar-link is-active link="#">
          <router-link to="/">Home</router-link>
        </fwb-navbar-link>
        <fwb-navbar-link link="">
          <router-link to="/about">About</router-link>
        </fwb-navbar-link>
        <fwb-navbar-link link="#">undefined</fwb-navbar-link>
        <fwb-navbar-link link="#"> Contact </fwb-navbar-link>
      </fwb-navbar-collapse>
    </template>
    <template #menu-icon>
      <svg
        class="w-6 h-6"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
        />
      </svg>
    </template>
  </fwb-navbar>
</template>

<style scoped></style>
