<template>
    <header>
        <div class="wrapper">
            <div class="row">
                <ApplicationLogo />
                <MainNavigationComponent />
            </div>
        </div>
    </header>
</template>

<script setup>
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import MainNavigationComponent from '@/Components/MainNavigationComponent.vue';
</script>

<style lang="scss" scoped>
    header {
        padding: 30px 0;
        .wrapper {
            max-width: 1440px;
            margin: 0 auto;
            padding: 0 40px;
            .row {
                display: flex;
                justify-content: space-between;
            }
        }
    }
</style>