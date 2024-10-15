<script setup>
import { themeColor, siteName } from "../data/items";
</script>
<template>
  <nav class="site-nav dark js-site-navbar mb-5 site-navbar-target">
    <div class="container">
      <div class="site-navigation">
        <a href="" class="logo m-0 float-left"
          ><div style="max-width: auto; height: auto;">
          <img src="" />
          </div> </a
        >
        <ul class="js-clone-nav d-none d-lg-inline-block site-menu float-left">
          <li class="active">
            <a href="#home-section" class="nav-link">Beranda</a>
          </li>
          <li class="has-children">
            <a href="#" class="nav-link">Berita</a>
            <ul class="dropdown">
              <li>
                <a href="#testimonials-section" class="nav-link"
                  >Agustus</a
                >
              </li>
              <li><a href="#" class="nav-link">September</a></li>
              <li><a href="#" class="nav-link">Oktober</a></li>
            </ul>
          </li>
          <li><a href="#features-section" class="nav-link">Profil</a></li>
          <li><a href="#pricing-section" class="nav-link">Kegiatan</a></li>
          <li><a href="#about-section" class="nav-link">Kurikulum</a></li>
          <li><a href="#contact-section" class="nav-link">PPDB 2024</a></li>
        </ul>
        <ul
          class="js-clone-nav d-none mt-1 d-lg-inline-block site-menu float-right"
        >
          <li class="cta-button-outline" style="margin-right: 1px;"><a href="#">Radio Spensev</a></li>
          <li class="cta-primary">
            <a href="#" :style="[{ backgroundColor: themeColor }]">Hubungi Kami</a>
          </li>
        </ul>
        <a
          href="#"
          class="burger ml-auto float-right site-menu-toggle js-menu-toggle d-inline-block dark d-lg-none"
          data-toggle="collapse"
          data-target="#main-navbar"
        >
          <span></span>
        </a>
      </div>
    </div>
  </nav>
</template>
