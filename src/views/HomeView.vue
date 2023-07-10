<template>
  <LandingPage />
  <br />
  <br />
  <BannerComponent />
  <br />
  <br />
<TestimonialVue />
<LoadSpinnerComponent/>
</template>

<script>
import LandingPage from '@/components/LandingPage.vue';
import BannerComponent from '@/components/BannerComponent.vue';
import TestimonialVue from '@/components/TestimonialVue.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
  components: {
    TestimonialVue,
    LandingPage,
    BannerComponent,
    LoadSpinnerComponent
  }
}

</script>