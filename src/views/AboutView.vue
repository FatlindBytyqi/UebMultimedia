<template>
  <AboutBanner />
  <br />
  <WhyChooseUsVue />
  <br />
  <WhoAreWeVue />
  <br />
  <AboutOurServicesSection />
<LoadSpinnerComponent/>

</template>

<script>
import AboutBanner from '@/components/AboutBanner.vue';
import WhyChooseUsVue from '@/components/WhyChooseUs.vue';
import WhoAreWeVue from '@/components/WhoAreWe.vue';
import AboutOurServicesSection from '@/components/AboutOurServicesSection.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
  components: {
    AboutBanner,
    WhyChooseUsVue,
    WhoAreWeVue,
    AboutOurServicesSection,
    LoadSpinnerComponent
  }
}

</script>
