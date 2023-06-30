<template>
  <WhyChooseUsVue />
  <br />
  <AboutBanner />
  <br />
  <WhoAreWeVue />
  <br />
  <AboutOurServicesSection />
<LoadSpinnerComponent/>

</template>

<script>
import WhyChooseUsVue from '@/components/WhyChooseUs.vue';
import WhoAreWeVue from '@/components/WhoAreWe.vue';
import AboutBanner from '@/components/AboutBanner.vue';
import AboutOurServicesSection from '@/components/AboutOurServicesSection.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
  components: {
    WhyChooseUsVue,
    WhoAreWeVue,
    AboutBanner,
    AboutOurServicesSection,
    LoadSpinnerComponent
  }
}

</script>
