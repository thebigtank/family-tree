<template>
    <button :class="['btn', type]">
        <slot />
    </button>
</template>

<script setup>

const props = defineProps({
    type: Array
});
</script>

<style lang="scss" scoped>

.btn {
    padding: 14px 30px;
    text-transform: capitalize;
    border-radius: 8px;
    font-weight: 600;
    transition: background-color 200ms ease-in-out;
    &.primary {
        background-color: #0145ff;
        color: #fff;

        &:hover {
            background-color: #15138f;
        }
    }

    &.secondary {
        background-color: #fff;
        color: #0145ff;

        &:hover {
            background-color: #0145ff;
            color: #fff;
        }
    }

    &.outline {
        border: 2px solid #0145ff;
        outline-style: unset;
        color: #0145ff;

        &:hover {
            background-color: #0145ff;
            color: #fff;
        }
    }
}
</style>
