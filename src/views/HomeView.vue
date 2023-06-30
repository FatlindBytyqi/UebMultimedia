<template>
  <LandingPage />
  <br />
  <br />
  <BannerComponent />
  <br />
  <br />
<TestimonialVue />
</template>

<script>
import TestimonialVue from '@/components/TestimonialVue.vue';
import LandingPage from '@/components/LandingPage.vue';
import BannerComponent from '@/components/BannerComponent.vue';


export default {
  components: {
    TestimonialVue,
    LandingPage,
    BannerComponent,
  }
}

</script>