<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <footer>
        <div class="container foot-flex">
            <div class="lists">
                <ul>
                    <h3>DC COMICS</h3>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <h3>SHOP</h3>
                    <li>link</li>
                    <li>link</li>

                </ul>

            </div>
        </div>
        <div class="social-link"></div>
    </footer>
</template>

<style scoped>
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    position: relative;
}

.social-link {
    width: 100%;
    height: 80px;
    background-color: #303030;
    position: absolute;
    bottom: 0;
}

.foot-flex {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

/*...*/
</style>