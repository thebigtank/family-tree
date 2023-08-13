<template>
    <Head title="Home" />

    <Header />
    <PricingPlan />
    <Services />

</template>

<script setup>
import { Head } from '@inertiajs/vue3';
import Header from '@/Components/HeaderComponent.vue';
import PricingPlan from '@/Components/PricingPlanComponent.vue';
import Services from '@/Components/ServicesComponent.vue';

</script>

<style lang="scss" scoped>
</style>
