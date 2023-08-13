<template>
    <li class="item">
        <ion-icon :name="icon"></ion-icon>
        <span>
            <slot></slot>
        </span>
    </li>
</template>

<script setup>

defineProps(['icon'])

</script>