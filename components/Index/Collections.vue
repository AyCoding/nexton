<script setup>
import {MoveRight} from 'lucide-vue-next';
</script>

<template>
    <div class="collections-section" style="max-width: 1536px; margin: auto">
        <div class="collection">
            <h2 style="font-size: 40px">
                Start exploring.
                <span style="color: var(--body-text-color); opacity: .8">Good things are waiting for you</span>
            </h2>

            <div class="collections-list">

                <div class="collection-card">
                    <div class="card-info">
                        <div class="title-group">
                            <h3>For Men's</h3>
                            <p>Starting at $24</p>
                        </div>
                        <NuxtLink href="/">
                            <div class="shop-link">
                                Shop Now
                                <MoveRight/>
                            </div>
                        </NuxtLink>
                    </div>
                </div>

                <div class="collection-card">
                    <div class="card-info">
                        <div class="title-group">
                            <h3>For Women's</h3>
                            <p>Starting at $19</p>
                        </div>
                        <NuxtLink href="/">
                            <div class="shop-link">
                                Shop Now
                                <MoveRight/>
                            </div>
                        </NuxtLink>
                    </div>
                </div>

                <div class="collection-card">
                    <div class="card-info">
                        <div class="title-group">
                            <h3>Accessories</h3>
                            <p>Explore accessories</p>
                        </div>
                        <NuxtLink href="/">
                            <div class="shop-link">
                                Shop Now
                                <MoveRight/>
                            </div>
                        </NuxtLink>
                    </div>
                </div>

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
</template>

<style scoped lang="scss">
.collections-section {
    padding-block: 88px;
    padding-inline: 120px;

    .collection {
        display: flex;
        flex-direction: column;
        gap: 40px;

        .collections-list {
            display: flex;
            gap: 20px;

            .collection-card {
                width: 100%;

                display: flex;
                gap: 10px;


                padding: 40px;

                background: var(--gray-bg);

                border-radius: 16px;

                .card-info {
                    display: flex;
                    width: 100%;
                    justify-content: space-between;
                }

                .title-group {
                    p {
                        font-size: 20px;
                        font-weight: 400;
                        color: var(--body-text-color);
                        line-height: 20px;
                    }
                }

                // TODO: REFACTO 
                .shop-link {
                    display: flex;
                    align-items: center;

                    gap: 8px;
                    padding-left: 12px;
                    padding-block: 8px;
                    text-transform: uppercase;

                    font-size: 14px;
                    font-weight: 500;
                    line-height: 20px;

                    color: var(--body-text-color)
                }

                a {
                    text-decoration: none;

                    &:visited {
                        color: inherit;
                    }
                }

                // TODO: REFACTO /\
                .shop-link {
                    border-left: 3px solid var(--border-color);

                    &:hover, &:hover svg {
                        color: var(--primary-color);
                    }

                    svg {
                        color: var(--body-text-color);
                    }
                }
            }
        }

        .slider-items {
            display: flex;
            justify-content: center;
            gap: 6px;

            padding-top: 40px;

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
    }
}
</style>