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
import AboutBanner from '@/components/About/AboutBanner.vue';
import WhyChooseUsVue from '@/components/About/WhyChooseUs.vue';
import WhoAreWeVue from '@/components/About/WhoAreWe.vue';
import AboutOurServicesSection from '@/components/About/AboutOurServicesSection.vue';
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
