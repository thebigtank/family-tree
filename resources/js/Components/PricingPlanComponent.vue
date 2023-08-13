<template>
    <section class="pricing-plan">
        <div class="wrapper">
            <div class="content">
                <h1 class="large-heading">Increase Your Payment Businesses of All Sizes.</h1>
                <span class="label">
                    Choose the plan that works best for you, feel free to contact us.
                </span>
            </div>

            <PricingPlanTab :is-monthly-billing="isMonthlyBilling" @update:is-monthly-billing="updateBilling" />
            <Plans :is-monthly-billing="isMonthlyBilling" :pricing-plans="pricingPlans" />
        </div>
    </section>
</template>

<script setup>
import PricingPlanTab from './PricingPlanTabComponent.vue';
import Plans from './PlansComponent.vue';
import { ref } from 'vue';

let isMonthlyBilling = ref(true);

const pricingPlans = [
    {
        title: 'silver',
        monthlyPrice: 9.99,
        annualPrice: 109.99,
        benefits: [
            'Free payment to other Pay accounts',
            '25 free local transfers',
            'Free ATM withdrawals in USD',
            '5 free international transfers fee'
        ],
        desc: 'Start your business with a simple account to manage it.',
    },
    {
        title: 'platinum',
        monthlyPrice: 49.99,
        annualPrice: 549.99,
        discount: '20',
        benefits: [
            'Free payment to other Pay accounts',
            'Unlimited free local transfers',
            'Free ATM withdrawals in USD & Euros',
            'Unlimited International transfers fee',
            'Priority 24/7 support',
            'Virtual card payment'
        ],
        desc: 'Available for businesses with large payments business models.',
    }
];

const updateBilling = (newValue) => {
    isMonthlyBilling.value = newValue;
};

</script>

<style lang="scss" scoped>
/* Add your scoped styles here */
</style>
