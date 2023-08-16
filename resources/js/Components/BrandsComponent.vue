<template>
    <section class="brands-block">
        <div class="wrapper">
            <div class="heading">
                <span class="label">
                    More than 50+ brands trusted using pay
                </span>
            </div>

            <div class="brands">
                <figure class="image">
                    <img src="https://ismachco.sirv.com/logos/SurrealDB.svg" alt="">
                </figure>
                <figure class="image">
                    <img src="https://ismachco.sirv.com/logos/Kubeshop.svg" alt="">
                </figure>
                <figure class="image">
                    <img src="https://ismachco.sirv.com/logos/Gupshup.svg" alt="">
                </figure>
                <figure class="image">
                    <img src="https://ismachco.sirv.com/logos/Proton.svg" alt="">
                </figure>
                <figure class="image">
                    <img src="https://ismachco.sirv.com/logos/Twilio.svg" alt="">
                </figure>
            </div>
        </div>
    </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.brands-block {
    padding: 80px 0;

    .wrapper {
        max-width: 1220px;
        margin: 0 auto;
        padding: 0 40px;
        overflow: hidden;

        .heading {
            margin: 0 auto;
            text-align: center;
            margin-bottom: 40px;

            .label {
                font-size: 20px;
                font-weight: 500;
                color: #8695ad;
            }
        }

        .brands {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 60px;
            .image {
                width: 180px;
                img {
                    width: 100%;
                    filter: grayscale(1);
                    opacity: 0.65;
                    cursor: pointer;
                    transition: all 250ms ease-in-out;

                    &:hover {
                        filter: grayscale(0);
                        opacity: 1;
                    }
                }
            }
        }
    }
}
</style>