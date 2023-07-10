<template>
    <ServiceBanner />
    <br />
    <OurServices />
<LoadSpinnerComponent/>

</template>

<script>
import ServiceBanner from '@/components/ServiceBanner.vue';
import OurServices from '@/components/OurServices.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
    components: {
        OurServices,
        ServiceBanner,
    LoadSpinnerComponent
    }
}

</script>