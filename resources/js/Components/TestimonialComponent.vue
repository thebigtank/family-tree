<template>
    <section class="testimonials">
        <div class="wrapper">
            <div class="row">
                <div class="col">
                    <figure class="image">
                        <img src="https://ismachco.sirv.com/Images/avatar-2.jpg" alt="">
                    </figure>
                </div>
                <div class="testimonial-content">
                    <swiper-container 
                    ref="swiperContainer"
                    :class="['swiper-container']"
                    :slides-per-view="1" 
                    :speed="500" 
                    :pagination="{ clickable: true }"
                    :allow-touch-move="true"
                    :loop="true" 
                    :autoplay="true" 
                    :css-mode="true" init="false">
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="content">
                                <span class="label">customer story</span>
                                <h2 class="title">
                                    <span>excellent payment service</span>
                                    <span>you guys are the best!</span>
                                </h2>
                                <blockquote>I like Pay more and more easch day because it makes my life a lot easier. Pay is worth much more then I paid. I can't say enough about Pay</blockquote>
                                <div class="customer">
                                    <figure class="avatar">
                                        <img src="https://ismachco.sirv.com/Images/avatar-4.jpg" alt="">
                                    </figure>
                                    <div class="content">
                                        <span class="name">arthur james</span>
                                        <span class="role">marketing manager - nike</span>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                    </swiper-container>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { register } from 'swiper/element/bundle';
import { ref, onMounted } from 'vue';

register();


const swiperContainer = ref(null);

onMounted(() => {
    const swiperEl = swiperContainer.value;
    const params = {
        injectStyles: [
            `
                .swiper-pagination {
                    text-align: left;
                }
            `,
        ],
    };

    Object.assign(swiperEl, params);

    swiperEl.initialize();
});

</script>

<style lang="scss" scoped>

</style>