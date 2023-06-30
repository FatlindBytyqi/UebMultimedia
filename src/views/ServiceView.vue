<template>
    <ServiceBanner />
    <br />
    <OurRooms />
</template>

<script>
import OurRooms from '@/components/OurRooms.vue';
import ServiceBanner from '@/components/ServiceBanner.vue';

export default {
    components: {
        OurRooms,
        ServiceBanner
    }
}

</script>