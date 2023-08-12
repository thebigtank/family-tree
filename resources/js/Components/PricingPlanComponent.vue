<template>
    <section class="pricing-plan">
        <div class="wrapper">
            <div class="content">
                <h1 class="large-heading">increase your payment businesses of all sizes.</h1>
                <span class="label">Choose the plan that works best for you, feel free to contact us.</span>
            </div>
            
            <PricingPlanTabComponent :isMonthlyBilling="isMonthlyBilling" @update:isMonthlyBilling="updateBilling" />
            <PlansComponent :isMonthlyBilling="isMonthlyBilling" />
        </div>
    </section>
</template>

<script setup>
import PricingPlanTabComponent from './PricingPlanTabComponent.vue';
import PlansComponent from './PlansComponent.vue';
import { ref } from 'vue';

let isMonthlyBilling = ref(true);

const updateBilling = (newValue) => {
    isMonthlyBilling.value = newValue;
};


</script>

<style lang="scss" scoped>

</style>