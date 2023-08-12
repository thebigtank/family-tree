<template>
    <nav>
        <ul>
            <li><a href="#">home</a></li>
            <li><a href="#">benefits</a></li>
            <li><a href="#">pricing</a></li>
            <li><a href="#">blog</a></li>
            <li><a href="#">login</a></li>
        </ul>
        <ButtonComponent :type="['outline']">get started</ButtonComponent>
    </nav>
</template>

<script setup>

import ButtonComponent from './ButtonComponent.vue';

</script>

<style lang="scss" scoped>
nav {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 40px;

    ul {
        display: flex;
        gap: 46px;

        li {
            a {
                display: block;
                text-transform: capitalize;
                font-size: 16px;
                font-weight: 600;
                color: #41557b;
                transition: color 200ms ease-in-out;

                &:hover {
                    color: #0145ff;
                }
            }
        }
    }
}
</style>
