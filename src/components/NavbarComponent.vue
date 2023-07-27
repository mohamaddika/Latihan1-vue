<template>
  <Navbar>
    <template #logo>
      <NavbarLogo
        link="https://www.google.com/"
        alt="Flowbite logo"
        image-url="unnamed.jpg"
        class="hover:scale-125 transition-all"
      >
        JBM STORE
      </NavbarLogo>
    </template>
    <template #default="{ isShowMenu }">
      <NavbarCollapse :isShowMenu="isShowMenu">
        <NavbarLink isActive link="#">Home</NavbarLink>
        <NavbarLink link="#">About</NavbarLink>
        <NavbarLink link="#">Contact</NavbarLink>
      </NavbarCollapse>
    </template>
  </Navbar>
</template>

<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue';
</script>
