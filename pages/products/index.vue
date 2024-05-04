<script setup></script>

<template>
    <main>
        <div class="main-content">
            <div class="product-content">
                <div class="product-info">
                    <div class="product-images">
                        <div class="images">
                            <img src="" alt="">
                            <img src="" alt="">
                            <img src="" alt="">
                            <img src="" alt="">
                        </div>
                        <div class="image-showing">
                            <img src="" alt="">
                            <div class="tag"></div>
                            <div class="cart-btn"></div>
                        </div>
                    </div>
                    <hr>
                    <div class="product-details">
                        <div class="description">
                            <h2>Black Automatic Watch</h2>
                            <p>The St. Louis Meramec Canoe Company was founded by Alfred Wickett in 1922. Wickett had
previously worked for the Old Town Canoe Co from 1900 to 1914. Manufacturing of the classic
wooden canoes in Valley Park, Missouri ceased in 1978.</p>
                        </div>
                        <div class="fabric">
                            <h2>Fabric + Care</h2>
                            <p>Material: Soft wool blend</p>
                            <p>Color: Various</p>
                        </div>
                        <div class="sales"></div>
                        <div class="keywords"></div>
                    </div>
                </div>
                <div class="add-to-cart">
                    <div class="sticky-container">
                        <div class="sticky">
                            <div class="price-container"></div>
                            <div class="size-container"></div>
                            <div class="quantity"></div>
                            <div class="total-price-info"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="recommendation-section">
                <div class="recommendations">
                    <h2></h2>
                    <div></div>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
main {
    max-width: 1536px;
    width: 100%;
    margin: auto;
    padding-inline: 120px;

    padding-top: 40px;
    padding-bottom: 72px;


    .main-content {
        display: flex;
        flex-direction: column;
        gap: 96px;
        padding-bottom: 24px;
    }
}


.product-content {
    display: flex;
    gap: 32px;
}

.product-info {
    display: flex;
    flex-direction: column;
    gap: 52px;
}

.product-details {
    display: flex;
    flex-direction: column;
    gap: 60px;


    p {
        font-size: 16px;
        font-weight: 400;
        line-height: 24px;
        color: var(--body-text-color);
    }
}


.add-to-cart {
    width: 460px;
    height: 105px;
    background: #ccc;
}
</style>