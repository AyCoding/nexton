<script setup>
import {Search} from 'lucide-vue-next'
</script>

<template>
    <div class="hero">
        <div class="hero-content">
            <div class="hero-slogan">
                <p style="font-weight: 500; font-size: 20px">Starting from: $49.99</p>

                <h1>Exclusive collection for everyone</h1>

                <NuxtLink href="/">
                    <div>
                        Explore now
                        <Search size="20"/>
                    </div>
                </NuxtLink>
            </div>

            <div class="hero-slider">
                <div></div>
                <div></div>
                <div></div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
.hero {
    position: relative;
    width: 100%;
    height: 600px;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("/hero-bg.jpg");
}


.hero-content {
    display: flex;
    align-items: center;

    max-width: 1536px;
    height: 100%;
    margin: auto;
    padding-inline: 120px;
}

.hero-slogan {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 632px;
    height: 100%;

    gap: 24px;
    padding-bottom: 20px;

    p {
        color: var(--body-text-color);
    }

    h1 {
        color: var(--primary-color);
    }
}


.hero-slogan a {
    text-decoration: none;
    font-size: 16px;
    font-weight: 500;
    width: fit-content;
}

.hero-slogan a div {
    display: flex;
    justify-content: center;
    align-items: center;
    background: var(--primary-color);
    padding: 20px 36px;
    width: 198px;
    color: #fff;
    border-radius: 9999px;
    transition: .3s;

    gap: 10px;

    &:hover {
        background: var(--body-text-color);
    }
}

.hero-slider {
    position: absolute;

    // A VERIFIER !!!
    max-width: 1296px;
    width: 100%;
    // A VERIFIER !!!

    display: flex;
    justify-content: center;
    padding-top: 24px;
    padding-bottom: 24px;
    gap: 12px;

    //    padding-inline: 120px;

    bottom: 0;
    
    
    div:first-child {
        width: 40px;
        height: 8px;
        background: var(--primary-color);
        opacity: 1;

    }

    div {
        border-radius: 30px;
        width: 8px;
        height: 8px;
        background: var(--primary-color);
        opacity: .8;
    }
}
</style>