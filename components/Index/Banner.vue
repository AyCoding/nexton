<script setup></script>

<template>
    <div class="banner-section">
        <div class="banner-container">
            <img src="/bg-image.jpg">
            <div class="banner-content">
                <div class="banner-body">
                    <div style="display: flex;flex-direction: column;gap: 14px; z-index: 100">
                        <p>100% Original Products</p>
                        <h2>The All New Fashion Collection Items</h2>
                    </div>
                    <p>Starting from: $59.99</p>


                    <NuxtLink href="/">
                        <div>Shop now</div>
                    </NuxtLink>
                </div>
            </div>
            
        </div>
    </div>
</template>

<style scoped lang="scss">
.banner-section {
    padding-inline: 120px;
    padding-block: 52px;

    max-width: 1536px;
    margin: auto;

    .banner-container {
        position: relative;
        background: #F5F5F5;
        border-radius: 24px;
        overflow: hidden;


        img {
            position: absolute;
            top: 0;
            right: 0;
            height: 100%;
            z-index: 0;
        }

        .banner-content {
            padding-block: 49px;
            padding-left: 120px;
            height: 437px;
            
            display: flex;
            align-items: center;
        }


        .banner-body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 24px;
            max-width: 552px;
        }
    }
}


a {
    text-decoration: none;
    font-size: 16px;
    font-weight: 500;
    width: fit-content;
}

a div {
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--primary-color);
    padding: 14px 32px;
    //    width: 198px;
    color: #fff;
    border-radius: 9999px;
    transition: .3s;
    font-size: 16px;
    font-weight: 500px;

    gap: 10px;

    &:hover {
        background: var(--body-text-color);
    }
}


p {
    color: var(--body-text-color);
    font-weight: 500;
    line-height: 20px;
}
</style>