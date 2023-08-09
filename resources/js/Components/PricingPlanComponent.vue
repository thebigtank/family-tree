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
        </div>
    </section>
</template>

<script setup>



</script>

<style lang="scss" scoped>

.pricing-plan {
    padding: 60px 0;
    .wrapper {
        max-width: 1220px;
        margin: 0 auto;
        .content {
            max-width: 700px;
            margin: 0 auto;
            text-align: center;
            margin-bottom: 80px;
            .large-heading {
                text-transform: capitalize;
                font-size: 58px;
                font-weight: 600;
                margin-bottom: 20px;
                line-height: 1.4;
                color: #142c5b;
            }

            .label {
                font-size: 18px;
                font-weight: 500;
                color: #8695ad;
            }
        }

        .pricing-tab {
            text-align: center;
            background-color: #eff6fc;
            padding: 8px;
            max-width: max-content;
            margin: 0 auto;
            border-radius: 16px;

            .btn {
                padding: 14px 30px;
                text-transform: capitalize;
                border-radius: 8px;
                font-weight: 600;
                transition: background-color 200ms ease-in-out;
                color: #41557b;

                // &:hover {
                //     background-color: #312fcb;
                //     color: #fff;
                // }

                &.active {
                    background-color: #ffffff;
                    color: #0145ff;
                }
            }
        }
    }
}

</style>