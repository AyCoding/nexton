<script setup></script>

<template>
    <footer>
        <div class="main-footer">
            <div class="footer-content">
                <div class="info">
                    <Logo/>

                    <div class="list">
                        <NuxtLink to="/">
                            <div class="list-item">Facebook</div>
                        </NuxtLink>
                        <NuxtLink to="/">
                            <div class="list-item">YouTube</div>
                        </NuxtLink>

                        <NuxtLink to="/">
                            <div class="list-item">Telegram</div>
                        </NuxtLink>
                        <NuxtLink to="/">
                            <div class="list-item">Twitter</div>
                        </NuxtLink>
                    </div>
                </div>

                <div class="getting-started">
                    <h5>Getting started</h5>

                    <div class="list">
                        <NuxtLink to="/">Release Notes</NuxtLink>
                        <NuxtLink to="/">Upgrade Guide</NuxtLink>
                        <NuxtLink to="/">Browser Support</NuxtLink>
                        <NuxtLink to="/">Dark Mode</NuxtLink>
                    </div>
                </div>

                <div class="explore">
                    <h5>Explore</h5>

                    <div class="list">
                        <NuxtLink to="/">Prototyping</NuxtLink>
                        <NuxtLink to="/">Design systems</NuxtLink>
                        <NuxtLink to="/">Pricing</NuxtLink>
                        <NuxtLink to="/">Security</NuxtLink>
                    </div>
                </div>

                <div class="community">
                    <h5>Community</h5>

                    <div class="list">
                        <NuxtLink to="/">Discussion Forums</NuxtLink>
                        <NuxtLink to="/">Code of Conduct</NuxtLink>
                        <NuxtLink to="/">Contributing</NuxtLink>
                        <NuxtLink to="/">API Reference</NuxtLink>
                    </div>
                </div>

            </div>
        </div>
        <div class="footer-bottom">
            <div class="footer-copyright">
                Nexton eCommerce. © 2024
            </div>
            <div class="payment-icons">
                VISA
                PAYPAL
                STRIPE
                VERISIGN
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">

footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    
    max-width: 1536px;
    width: 100%;
    margin: auto;
    padding-inline: 120px;


    .main-footer {
        padding-block: 60px;
        width: 100%;
    }

    .footer-content {
        display: flex;
        // width: 100%;

        a {
            font-size: 16px;
            font-weight: 400;
            line-height: 24px;
            color: var(--body-text-color);
            text-decoration: none;
            width: fit-content;


            &:visited {
                color: var(--body-text-color);
            }
        }

        .info, .getting-started, .explore, .community {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            gap: 20px;

            width: 100%;

            .list {
                display: flex;
                flex-direction: column;
                gap: 12px;
            }
        }
    }
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
    padding-block: 32px;

    font-size: 16px;
    line-height: 24px;
    font-weight: 400;
    color: var(--body-text-color);
}
</style>