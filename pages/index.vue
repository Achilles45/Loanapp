<template>
  <div class="app">
    <Navbar />
    <HeroSection />
    <Loan />
    <Features />
    <Appsection />
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import HeroSection from '~/components/HeroSection.vue'
import Loan from '~/components/Loan.vue'
import Features from '~/components/Features.vue'
import Appsection from '~/components/Appsection.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    HeroSection,
    Loan,
    Features,
    Appsection,
    Footer
  }
}
</script>