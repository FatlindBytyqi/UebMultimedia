<template>
  <WhyChooseUsVue />
  <br />
  <AboutBanner />
  <br />
  <WhoAreWeVue />
  <br />
  <AboutOurRoomSectionVue />
</template>

<script>
import WhyChooseUsVue from '@/components/WhyChooseUs.vue';
import WhoAreWeVue from '@/components/WhoAreWe.vue';
import AboutBanner from '@/components/AboutBanner.vue';
import AboutOurRoomSectionVue from '@/components/AboutOurRoomSection.vue';

export default {
  components: {
    WhyChooseUsVue,
    WhoAreWeVue,
    AboutBanner,
    AboutOurRoomSectionVue
  }
}

</script>
