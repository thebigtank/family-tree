<template>
    <section class="pricing-plan">
        <div class="wrapper">
            <div class="content">
                <h1 class="large-heading">increase your payment businesses of all sizes.</h1>
                <span class="label">Choose the plan that works best for you, feel free to contact us.</span>
            </div>

            <div class="pricing-tab">
                <button class="btn active">bill anually</button>
                <button class="btn">bill monthly</button>
            </div>

            <div class="pricing-plans">
                <div class="plan">
                    <div class="content-wrap">
                        <span class="plan__title">silver card</span>
                        <div class="price">
                            <sup>$</sup>
                            <span>9.99</span>
                        </div>
                        <span class="price-label">user per month</span>
                        <div class="credit-card">
                            <img src="https://www.transparentpng.com/thumb/credit-card/8p4jX1-blank-credit-card-pic.png" alt="Blank Credit Card Pic @transparentpng.com">
                        </div>
                        <span class="desc">Start your business with a simple account to manage it</span>
                        <hr>
                        <ul class="benefits">
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Free payment to other Pay accounts</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>25 free local transfers</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Free ATM withdrawals in USD</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>5 free international transfers fee</span>
                            </li>
                        </ul>
                        <ButtonComponent type="outline">get started</ButtonComponent>
                    </div>
                </div>
                <div class="plan">
                    <div class="content-wrap">
                        <span class="plan__title">platinum card</span>
                        <div class="price">
                            <sup>$</sup>
                            <span>9.99</span>
                        </div>
                        <span class="price-label">user per month</span>
                        <div class="credit-card">
                            <img src="https://www.transparentpng.com/thumb/credit-card/8p4jX1-blank-credit-card-pic.png" alt="Blank Credit Card Pic @transparentpng.com">
                        </div>
                        <span class="desc">Available for businesses with large payments business models</span>
                        <hr>
                        <ul class="benefits">
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Free payment to other Pay accounts</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Unlimited free local transfers</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Free ATM withdrawals in USD & Euros</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Unlimited International transfers fee</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Priority 24/7 support</span>
                            </li>
                            <li class="item">
                                <ion-icon name="checkmark-circle"></ion-icon>
                                <span>Virtual card payment</span>
                            </li>
                        </ul>
                        <ButtonComponent type="outline">get started</ButtonComponent>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import ButtonComponent from './ButtonComponent.vue';


</script>

<style lang="scss" scoped>

</style>