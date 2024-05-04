<script setup>
import {Search, UserRound, ShoppingCart} from 'lucide-vue-next'
</script>

<template>
    <header>
        <div class="hero-container">
            <div class="logo">
            <span style="font-weight: 600; font-size: 34px; letter-spacing: -1.84px">NEXTON</span>
            <span style="letter-spacing: -1.6px">eCommerce</span>
        </div>
        <div style="flex: 1; display: flex; justify-content: center;">
            <form action="" method="get">
                <div
                        style="background: var(--gray-bg); width: 352px; height: 52px; border-radius: 99999px;  display: flex; justify-content: center; align-items: center; padding: 0 24px; gap: 10px">
                        <button class="btn-search">
                            <Search size="20" style="color: var(--body-text-color);"/>
                        </button>
                        <input type="text" placeholder="Search in products..." name="q"
                            style="width: 100%; background: var(--gray-bg); outline: none; border: none; height: 20px; font-size: 14px; font-weight: 400;font-family: 'Poppins'; color: var(--body-text-color)">
                    </div>
            </form>
        </div>
        <div class="right" style="width: 78px;display: flex; justify-content: space-between;">
            <NuxtLink href="/">
                <UserRound/>
            </NuxtLink>
            <NuxtLink href="/">
                <div class="cart">
                    <ShoppingCart/>
                    <div class="total-of-cart">3</div>
                </div>
            </NuxtLink>
        </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
.hero-container {
    display: flex;
    align-items: center;
    padding-inline: 120px;
    height: 100px;
    max-width: 1536px;
    margin: auto;
}

.logo {
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
    padding: 0;
    text-align: right;
    color: var(--primary-color);
}

input {
    &::placeholder {
        color: var(--body-text-color);
    }
}

.cart {
    svg {
        color: var(--body-text-color);
        transition: .3s;
    }
}

.cart {
    position: relative;
    
    .total-of-cart {
        position: absolute;
        top: -10px;
        right: -10px;
        
        display: flex;
        justify-content: center;
        align-items: center;
        
      
        background: var(--vibrant-color);
        /*padding-inline: 5px;*/
        border-radius: 9999px;
        
        width: 20px;
        height: 20px;
        
        color: #fff;
        font-size: 12px;
        font-weight: 500;
    }
}

.btn-search {
    padding: 0;
    margin: 0;
    background: transparent;
    border: none;
    outline: none;
    transition: .3s;
}

.right a:visited {
    color: var(--body-text-color);
}

.right a {
    transition: .3s;
    
    &:hover {
        color: var(--primary-color);
    }
}
</style>