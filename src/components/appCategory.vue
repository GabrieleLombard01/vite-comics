<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="category">
        <div class="container">
            <ul class="nav-cat">
                <li>
                    <a class="items-center" href="#">
                        <img class="small_size" src="../assets/img/buy-comics-digital-comics.png" alt="cat1">
                        <span>DIGITAL COMICS</span>
                    </a>
                </li>
                <li>
                    <a class="items-center" href="#">
                        <img class="small_size" src="../assets/img/buy-comics-merchandise.png" alt="cat2">
                        <span>DC MERCHANDISE</span>

                    </a>
                </li>
                <li>
                    <a class="items-center" href="#">
                        <img class="small_size" src="../assets/img/buy-comics-subscriptions.png" alt="cat3">
                        <span>SUBSCRIPTION</span>

                    </a>
                </li>
                <li>
                    <a class="items-center" href="#">
                        <img class="small_size" src="../assets/img/buy-comics-shop-locator.png" alt="cat4">
                        <span>COMIC SHOP LOCATOR</span>

                    </a>
                </li>
                <li>
                    <a class="items-center" href="#">
                        <img class="small_size" src="../assets/img/buy-dc-power-visa.svg" alt="cat5">
                        <span>DC POWER VISA</span>

                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
.category {
    min-height: 130px;
    background-color: #0282f9;
    padding-top: 20px;
}

.nav-cat {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 40px;
}

.items-center {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}

/*...*/
</style>