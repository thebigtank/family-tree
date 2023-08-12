<template>
    <div class="pricing-tab">
        <button class="btn" :class="{ active: isMonthlyBilling }" @click="updateBilling(true)">bill monthly</button>
        <button class="btn" :class="{ active: !isMonthlyBilling }" @click="updateBilling(false)">bill anually</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const props = defineProps(['isMonthlyBilling']);
const emits = defineEmits();

let isMonthlyBilling = ref(true);

const updateBilling = (isMonthly) => {
    isMonthlyBilling.value = isMonthly;
    emits('update:isMonthlyBilling', isMonthly); // Emitting the value to the parent
};

</script>

<style lang="scss" scoped>

</style>