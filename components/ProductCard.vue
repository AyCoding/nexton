<template>
    <div class="product-card">
        <div class="product-image">
            <div class="cart-btn">
                <img src="/icons/cart-btn.svg" alt="">

            </div>
            <div class="tag"></div>
            <img src="/product-image.jpg" alt="">
        </div>

        <div class="product-info">
            <div class="info">
                <div class="info-content">
                    <h5>Black Automatic Watch</h5>
                    <p>
                        Accessories
                    </p>
                </div>
                <div class="rating">
                    <img src="/icons/star.svg" alt="">
                    <p>4.9 (98)</p>
                </div>
            </div>
            <div class="price">
                <h5>$169.99</h5>
                <span>$199.99</span>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
.rating {
    display: flex;
    align-items: center;
    gap: 4px;
}

p {
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    color: var(--body-text-color)
}

.product-card {
    display: flex;
    flex-direction: column;

    gap: 20px;

    //    width: 309px; // PAS DYNAMIQUE
    width: 100%;


    .product-image {
        position: relative;
        border-radius: 16px;

        > img {
            border-radius: 16px;
            width: 100%;

            object-fit: cover;
        }

        .cart-btn {
            top: 12px;
            right: 12px;
            position: absolute;
            padding: 10px;
            background: var(--default-bg);
            border-radius: 9999px;

            img {
                width: 16px;
                height: 16px;
            }
        }

    }

    .product-info {
        display: flex;
        justify-content: space-between;

        gap: 20px;
        padding-inline: 16px;

        .info {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .price {
            display: flex;
            flex-direction: column;
            align-items: flex-end;

            span {
                text-decoration: line-through;
                font-size: 14px;
                line-height: 20px;
                font-weight: 400;
            }
        }
    }
}
</style>