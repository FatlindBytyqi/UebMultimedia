<template>
    <ServiceBanner />
    <br />
    <OurServices />
<LoadSpinnerComponent/>

</template>

<script>
import OurServices from '@/components/OurServices.vue';
import ServiceBanner from '@/components/ServiceBanner.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';


export default {
    components: {
        OurServices,
        ServiceBanner,
    LoadSpinnerComponent
    }
}

</script>