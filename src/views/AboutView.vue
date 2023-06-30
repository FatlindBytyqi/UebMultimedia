<template>
  <WhyChooseUsVue />
  <br />
  <AboutBanner />
  <br />
  <WhoAreWeVue />
  <br />
  <AboutOurRoomSectionVue />
<LoadSpinnerComponent/>

</template>

<script>
import WhyChooseUsVue from '@/components/WhyChooseUs.vue';
import WhoAreWeVue from '@/components/WhoAreWe.vue';
import AboutBanner from '@/components/AboutBanner.vue';
import AboutOurRoomSectionVue from '@/components/AboutOurRoomSection.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
  components: {
    WhyChooseUsVue,
    WhoAreWeVue,
    AboutBanner,
    AboutOurRoomSectionVue,
    LoadSpinnerComponent
  }
}

</script>
