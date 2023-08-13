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

defineProps(['isMonthlyBilling','pricingPlans']);

</script>

<style lang="scss" scoped>

</style>