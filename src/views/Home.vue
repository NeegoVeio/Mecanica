<template>
  <div>
    <AppHeader />
    <MainNavbar />
    <HeroSection />
    <SobreNos />
    <ServicosSection />
    <FloatingSocial />
    <SiteFooter />
  </div>
</template>

<script>
import AppHeader from "@/components/Header.vue";
import MainNavbar from "@/components/Navbar.vue";
import HeroSection from "@/components/Hero.vue";
import SobreNos from "@/components/SobreNos.vue";
import ServicosSection from "@/components/Servicos.vue";
import FloatingSocial from "@/components/FloatingSocial.vue";
import SiteFooter from "@/components/Footer.vue";

export default {
  name: "HomeView",
  components: {
    AppHeader,
    MainNavbar,
    HeroSection,
    SobreNos,
    ServicosSection,
    FloatingSocial,
    SiteFooter,
  },
};
</script>
