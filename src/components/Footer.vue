<script setup>
import { contactInfo } from "../data/items";

const copyrightText = "SMP N 7 Semarang";
const column1Heading = "Tentang SMP Negeri 7 Semarang";
const column1Text =
  "SMPN 7 Semarang berkomitmen untuk menciptakan lingkungan belajar yang positif, di mana setiap siswa dihargai dan didorong untuk berkembang sesuai dengan karakter masing-masing.";
const column2Heading = "Fitur";
const column3Heading = "Organisasi";
const column4Heading = "Kontak";

const connectHeading = "Tautan";

const socialItems = [
  {
    link: "https://www.instagram.com/smpn7semarang/",
    icon: "icon-instagram",
  },
  {
    link: "https://twitter.com/smpn7semarang",
    icon: "icon-twitter",
  },
  {
    link: "https://www.facebook.com/spentura.jaya.79",
    icon: "icon-facebook",
  },
  {
    link: "https://www.youtube.com/channel/UC75GkU_4MmGQNyhpgAP_pOQ",
    icon: "icon-youtube",
  },
  {
    link: "http://wa.me//6281362454534",
    icon: "icon-whatsapp",
  },
];
</script>

<template>
  <div class="site-footer">
    <div class="footer-dots"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="widget">
            <h3>{{ column1Heading }}</h3>
            <p>{{ column1Text }}</p>
          </div>
          <div class="widget">
            <h3>{{ connectHeading }}</h3>
            <ul class="list-unstyled social">
              <li style="margin-right: 4px">
                <a :href="socialItems[0].link"
                  ><span :class="socialItems[0].icon"></span
                ></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[1].link"
                  ><span :class="socialItems[1].icon"></span
                ></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[2].link"
                  ><span :class="socialItems[2].icon"></span
                ></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[3].link"
                  ><span :class="socialItems[3].icon"></span
                ></a>
              </li>
              <li>
                <a :href="socialItems[4].link"
                  ><span :class="socialItems[4].icon"></span
                ></a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-lg-2 ml-auto">
          <div class="widget">
            <h3>{{ column2Heading }}</h3>
            <ul class="list-unstyled float-left links">
              <li><a href="#">Library Spentura</a></li>
              <li><a href="#">E-Mading</a></li>
              <li><a href="#">Galeri</a></li>
              <li><a href="#">Prestasi Siswa</a></li>
              <li><a href="#">Program Sekolah</a></li>
            </ul>
          </div>
        </div>
        <div class="col-lg-2">
          <div class="widget">
            <h3>{{ column3Heading }}</h3>
            <ul class="list-unstyled float-left links">
              <li><a href="#">Pramuka</a></li>
              <li><a href="#">OSIS</a></li>
              <li><a href="#">PMR</a></li>
              <li><a href="#">Ekstrakulikuler</a></li>
            </ul>
          </div>
        </div>
        <div class="col-lg-3">
          <div class="widget">
            <h3>{{ column4Heading }}</h3>
            <address>{{ contactInfo.address }}</address>
            <ul class="list-unstyled links mb-4">
              <li>
                <a :href="'tel://' + contactInfo.phone1">{{
                  contactInfo.phone1
                }}</a>
              </li>           
              <li>
                <a :href="'mailto:' + contactInfo.email"
                  ><span>{{ contactInfo.email }}</span></a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12 text-center">
          <p>
            {{ copyrightText }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
