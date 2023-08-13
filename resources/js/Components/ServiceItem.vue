<template>
    <div class="service-item">
        <span class="icon">
            <ion-icon :name="icon"></ion-icon>
        </span>
        <h3 class="service-title">{{ title }}</h3>
        <slot></slot>
    </div>
</template>

<script setup>

defineProps(['icon', 'title'])

</script>