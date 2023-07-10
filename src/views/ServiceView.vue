<template>
    <ServiceBanner />
    <br />
    <OurServices />
    <CaruselComponent/>
<LoadSpinnerComponent/>

</template>

<script>
import ServiceBanner from '@/components/Service/ServiceBanner.vue';
import OurServices from '@/components/Service/OurServices.vue';
import CaruselComponent from '@/components/Service/CaruselComponent.vue';
import LoadSpinnerComponent from '@/components/LoadSpinnerComponent.vue';

export default {
    components: {
        ServiceBanner,
        OurServices,
        CaruselComponent,
    LoadSpinnerComponent
    }
}

</script>