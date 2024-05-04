<script setup>
// TODO : Rename all class css

</script>

<template>
    <section class="bestsellers-section" style="max-width: 1536px; margin: auto">
        <div class="bestsellers">
            <h2 style="font-size: 40px">
                Best Sellers. 
                <span style="color: var(--body-text-color); opacity: .8">Best selling of the month</span>
            </h2>

            <div class="bestseller-products">
                <div class="products">
                    <ProductCard />
                    <ProductCard />
                    <ProductCard />
                    <ProductCard />
                </div>
                <div class="slider-items">
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                    <div></div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.bestsellers-section {
    padding-block: 88px;
    padding-inline: 120px;

    .bestsellers {
        display: flex;
        flex-direction: column;
        gap: 40px;
        
        
        .bestseller-products {
            .products {
                display: flex;
                gap: 20px;
            }
        }
    }
}


.slider-items {
    display: flex;
    justify-content: center;
    gap: 6px;

    padding-top: 64px;

    div {
        width: 6px;
        height: 6px;
        border-radius: 9999px;
        background: var(--primary-color);
        opacity: .5;
    }

    div:first-child {
        background: var(--primary-color);
        opacity: 1;
    }
}


</style>