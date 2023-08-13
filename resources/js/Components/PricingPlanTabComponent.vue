<template>
    <div class="pricing-tab">
        <button v-for="billingType in billingTypes" :key="billingType.id"
            :class="['btn', { 'active': isMonthlyBilling === billingType.isMonthly }]"
            @click="updateBilling(billingType.isMonthly)">
            {{ billingType.label }}
        </button>
    </div>
</template>

<script setup>
defineProps(['isMonthlyBilling']);
const emit = defineEmits(['update:is-monthly-billing']);

const billingTypes = [
    { id: 1, label: 'Bill Monthly', isMonthly: true },
    { id: 2, label: 'Bill Annually', isMonthly: false },
];

const updateBilling = (isMonthly) => {
    emit('update:is-monthly-billing', isMonthly);
};
</script>

<style lang="scss" scoped>
/* Add your scoped styles here */
</style>
