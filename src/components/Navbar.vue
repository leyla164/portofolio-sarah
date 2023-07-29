<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>
<template>
    <Navbar solid>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Flowbite logo" image-url="https://st3.depositphotos.com/6697918/15699/v/450/depositphotos_156995416-stock-illustration-beautiful-face-of-arabic-muslim.jpg">
           <h2>PORTFOLIO</h2>
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Halaman utama</NavbarLink>
          <NavbarLink>Beranda</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
          <NavbarLink>Kontak</NavbarLink>
        </NavbarCollapse>
      </template>
    </Navbar>
</template>