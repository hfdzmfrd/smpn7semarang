<script setup>
import mainPhoto from "../assets/images/hero.png";
import { themeColor } from "../data/items";

const heroHeading = "SMPN 7 SEMARANG SEKOLAH UNGGULAN";
const buttonSeeFeature = "Sambutan Kepala Sekolah";
const buttonPricing = "Program Unggulan";
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="dots"></div>
          <div class="row align-items-center">
            <div
              class="col-lg-7 ml-auto order-lg-2"
              data-aos="fade-right"
              data-aos-delay="400"
            >
              <img :src="mainPhoto" alt="Image" class="img-fluid" />
            </div>
            <div class="col-lg-5">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">
                {{ heroHeading }}
              </h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p>
                  SMP NEGERI 7 Semarang memiliki kurikulum yang inovatif, pengajaran yang berfokus pada pengembangan karakter, serta fasilitas yang mendukung kegiatan belajar mengajar. 
                  Selain itu, para guru kami adalah tenaga profesional yang berdedikasi, siap memberikan bimbingan optimal kepada setiap siswa. Dengan berbagai ekstrakurikuler yang beragam,
                  kami juga menanamkan nilai kerja sama dan kepemimpinan sejak dini. Semua ini menjadikan sekolah kami tempat yang ideal untuk membentuk generasi yang berkualitas.
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <a
                  href="#features-section"
                  class="btn btn-primary smoothscroll"
                  style="margin-right: 5px"
                  :style="[
                    { background: themeColor },
                    { borderColor: themeColor },
                  ]"
                  >{{ buttonSeeFeature }}</a
                >
                <a
                  href="#"
                  class="btn btn-outline-primary smoothscroll pricing"
                  :style="[{ color: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonPricing }}</a
                >
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pricing:hover {
  color: #fff !important;
}
</style>
