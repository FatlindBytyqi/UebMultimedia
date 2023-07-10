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
import LandingPage from '@/components/Home/LandingPage.vue';
import BannerComponent from '@/components/Home/BannerComponent.vue';
import TestimonialVue from '@/components/Home/TestimonialVue.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
  components: {
    LandingPage,
    BannerComponent,
    TestimonialVue,
    LoadSpinnerComponent
  }
}

</script>