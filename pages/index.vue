<script setup>
import {Truck, Recycle, Globe, CircleDollarSign} from 'lucide-vue-next'
</script>

<template>
    <IndexHero />
    <div class="brand-info" style="max-width: 1536px; margin: auto">
        <div class="brand-info-content">
            <section>
                <Truck/>
                <div>
                    <h4>Free shipping</h4>
                    <p>On orders over $50.00</p>
                </div>
            </section>
            <section>
                <Recycle/>
                <div>
                    <h4>Very easy to return</h4>
                    <p>Just phone number</p>
                </div>
            </section>
            <section>
                <Globe/>
                <div>
                    <h4>Worldwide delivery</h4>
                    <p>Fast delivery worldwide</p>
                </div>
            </section>
            <section>
                <CircleDollarSign/>
                <div>
                    <h4>Refunds policy</h4>
                    <p>60 days return for any reason</p>
                </div>
            </section>
        </div>
    </div>

    <IndexCollections/>
    <IndexRecommendation/>
    <IndexBestsellers/>
    <IndexBanner/>
</template>

<style scoped lang="scss">
.brand-info {
    padding-inline: 120px;
    padding-top: 52px;
    padding-bottom: 32px;

    .brand-info-content {
        border: 1px solid var(--border-color);
        padding: 24px 40px;
        border-radius: 16px;

        display: flex;

        section {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 16px;
            margin: auto;

            svg {
                min-width: 24px;
                min-height: 24px;
                color: var(--primary-color);
            }

            div {
                // width: 100%;
                display: flex;
                flex-direction: column;
                gap: 2px;
                padding-inline: 32px;

                border-right: 1px solid var(--border-color);


            }

            &:last-child div {
                border: none
            }

            p {
                color: var(--body-text-color);
                font-size: 14px;
                font-weight: 400;
            }
        }
    }
}
</style>