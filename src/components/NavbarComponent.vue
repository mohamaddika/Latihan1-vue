<template>
  <Navbar>
    <template #logo>
      <NavbarLogo
        link="https://www.google.com/"
        alt="Flowbite logo"
        image-url="https://yt3.googleusercontent.com/ytc/AOPolaQgNDqfxvXBJ48RUMR7Rbt63HFc86m_6OGO6Y7tgQ=s900-c-k-c0x00ffffff-no-rj"
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
