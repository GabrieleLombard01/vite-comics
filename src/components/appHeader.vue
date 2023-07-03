<script>
export default {
    data() {
        return {
            navbarLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],
        }
    }
}
</script>

<template>
    <header>
        <div class="container flex-header">
            <!--LOGO:-->
            <figure>
                <img src="../assets/img/dc-logo.png" alt="logo">
            </figure>
            <!--NAV:-->
            <ul class="top-navbar">
                <li v-for="link in navbarLinks" :key="link.text" :class="{ 'current-link': link.current }">
                    <strong>{{ link.text }}</strong>
                </li>
            </ul>
        </div>
    </header>
</template>

<style scoped>
.flex-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

.flex-header li:hover {
    border-bottom: solid #0282f9 2px;
    cursor: pointer;
}



/*NAV*/
.top-navbar {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    padding-right: 40px;
}

.top-navbar li {
    font-size: 20px;
}
</style>