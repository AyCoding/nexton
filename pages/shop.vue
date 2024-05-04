<script setup>

</script>

<template>
    <main class="main">
        <div class="main-content">
            <div class="sidebar-container">
                <div class="sidebar">
                    <div class="categories">
                        <h4>Categories</h4>

                        <div class="category-list">

                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Men’s fashion</label>
                            </div>

                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Women’s fashion</label>
                            </div>

                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Kids & Toys</label>
                            </div>
                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Accessories</label>
                            </div>
                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Cosmetics</label>
                            </div>
                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Shoes</label>
                            </div>
                            <div class="checkbox">
                                <input type="checkbox">
                                <label for="">Sports</label>
                            </div>
                        </div>
                    </div>
                    <div class="price">
                        <h4>Price range</h4>

                            <div class="price-range">
                                <div class="price-slider">
                                    <input type="range" name="" id="" style="width: 100%;"
                                </div>
                                <div class="price-inputs">
                                    <div class="min-price-input">
                                        <p>Min price</p>
                                        <div class="input">
                                            <input type="text" value="100"> <span>$</span>
                                        </div>
                                    </div>
                                    <div class="max-price-input">
                                        <p>Max price</p>
                                        <div class="input">
                                           <input type="text" value="500"> <span>$</span>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    <div class="sorting">
                        <h4>Sort order</h4>

                        <div class="sorting-list">
                            <div class="radio">
                                <input type="radio" name="sort">
                                <label for="">Most Popular</label>
                            </div>
                            <div class="radio">
                                <input type="radio" name="sort">
                                <label for="">Best Rating</label>
                            </div>
                            <div class="radio">
                                <input type="radio" name="sort">
                                <label for="">Newest</label>
                            </div>
                            <div class="radio">
                                <input type="radio" name="sort">
                                <label for="">Price Low - Hight</label>
                            </div>
                            <div class="radio">
                                <input type="radio" name="sort">
                                <label for="">Price Hight - Low</label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="products-container">
                <div class="products">
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                    <ProductCard/>
                </div>
                <div class="pagination"></div>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
.main {
    max-width: 1536px;
    margin: auto;

    padding-top: 40px;
    padding-bottom: 72px;

    .main-content {
        display: flex;
        gap: 20px;
    }
}

.sidebar-container {
    // background: rgb(0, 60, 255);
    max-width: 309px;
    width: 100%;
    height: 500px; // 100%

    .sidebar {
        display: flex;
        flex-direction: column;
        gap: 32px;

        .categories {
            padding-bottom: 40px;
            border-bottom: 1px solid var(--border-color);

            .category-list {
                display: flex;
                flex-direction: column;
                gap: 16px;
                padding-top: 16px;

                .checkbox {
                    display: flex;
                    align-items: center;
                    gap: 12px;
                    font-size: 14px;
                    font-weight: 400;
                    line-height: 20px;
                    
                    input[type=checkbox] {
                        width: 20px;
                        height: 20px;
                        border-radius: 4px;
                        border: 1px solid #000;
                    }
                }
            }
        }
        .price {
            display: flex;
            flex-direction: column;
            gap: 24px;
            padding-bottom: 40px;
            border-bottom: 1px solid var(--border-color);

            .price-range {
                display: flex;
                flex-direction: column;
                gap: 20px;
            }

            .price-inputs {
                display: flex;
                gap: 24px;
                width: 100%;
                color: var(--body-text-color);

                .input {
                    position: relative;
                    display: flex;
                    align-items: center;
                    font-weight: 500;


                    input {
                        width: min-content;
                        padding-block: 8px;
                        padding-inline: 16px;
                        border-radius: 9999px;
                        width: 100%;
                        outline: none;
                        border: 1px solid var(--border-color);
                        color: var(--body-text-color);
                        font-family: 'Poppins', sans-serif;
                        font-weight: 500;
                    }

                    span {
                        position: absolute;
                        right: 16px;
                    }
                }

                .min-price-input,.max-price-input {
                    display: flex;
                    flex-direction: column;
                    gap: 4px;
                    width: 100%;
                }
            }
        }
    }
}



.sorting {
            padding-bottom: 40px;
            border-bottom: 1px solid var(--border-color);

            .sorting-list {
                display: flex;
                flex-direction: column;
                gap: 16px;
                padding-top: 16px;

                .radio {
                    display: flex;
                    align-items: center;
                    gap: 12px;
                    font-size: 14px;
                    font-weight: 400;
                    line-height: 20px;
                    
                    input[type=radio] {
                        width: 20px;
                        height: 20px;
                        border-radius: 4px;
                        border: 1px solid #000;
                    }
                }
            }
        }


.products-container {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 52px;

    .products {
        display: flex;
        flex-wrap: wrap;

        gap: 52px 20px;

        .product-card {
            display: flex;
            flex-wrap: wrap;
            max-width: 309px;
        }
    }
}
</style>