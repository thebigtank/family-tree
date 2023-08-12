<template>

    <div class="pricing-plans">
        <div v-for="(plan, index) in pricingPlans" :key="index" class="plan" :class="{ discounted: !isMonthlyBilling && plan.discount }">
            <div class="plan-card">
                <div class="card">
                    <span v-if="!isMonthlyBilling && plan.discount" class="discount-label">save {{ plan.discount }}%</span>
                    <span class="plan__title">{{ plan.title }} card</span>
                    <div class="price">
                        <sup>$</sup>
                        <span v-if="isMonthlyBilling">{{ plan.monthlyPrice }}</span>
                        <span v-else>{{ plan.annualPrice }}</span>
                    </div>
                    <span v-if="isMonthlyBilling" class="price-label">usd per month</span>
                    <span v-else class="price-label">usd per year</span>
                    <div class="credit-card">
                        <img src="https://www.transparentpng.com/thumb/credit-card/8p4jX1-blank-credit-card-pic.png" alt="Blank Credit Card Pic @transparentpng.com">
                    </div>
                    <span class="desc">{{ plan.desc }}</span>
                    <hr>
                    <ul class="benefits">
                        <li v-for="(item, index) in plan.benefits" :key="index" class="item">
                            <ion-icon name="checkmark-circle"></ion-icon>
                            <span>{{ item }}</span>
                        </li>
                    </ul>
                    <ButtonComponent :type="['outline']">get started</ButtonComponent>
                </div>
            </div>
            <span v-if="!isMonthlyBilling && plan.discount" class="discount-message">*Limited offer, save {{ plan.discount }}% for annual plan {{ plan.title }} card.</span>
        </div>
    </div>
</template>

<script setup>
import ButtonComponent from './ButtonComponent.vue';

const props = defineProps({
    isMonthlyBilling: Boolean,
});

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
</script>

<style lang="scss" scoped>

</style>