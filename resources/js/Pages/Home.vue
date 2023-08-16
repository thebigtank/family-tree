<template>
    <Head title="Home" />

    <Header />
    <PricingPlan />
    <Services />
    <Brands />
    <Testimonials />

</template>

<script setup>
import { Head } from '@inertiajs/vue3';
import Header from '@/Components/HeaderComponent.vue';
import PricingPlan from '@/Components/PricingPlanComponent.vue';
import Services from '@/Components/ServicesComponent.vue';
import Brands from '@/Components/BrandsComponent.vue';
import Testimonials from '@/Components/TestimonialComponent.vue';

</script>

<style lang="scss" scoped>
</style>
