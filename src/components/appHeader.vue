<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <header>
        <!--LOGO:-->
        <figure>
            <img src="../assets/img/dc-logo.png" alt="logo">
        </figure>
        <!--NAV:-->
        <ul class="top-navbar">
            <li>link</li>
            <li>link</li>
            <li>link</li>
            <li>link</li>
            <li>link</li>
        </ul>
    </header>
</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

/*NAV*/
.top-navbar {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    padding-right: 40px;
}
</style>