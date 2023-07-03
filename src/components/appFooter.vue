<script>
export default {
    data() {
        return {
            footerLinks: [
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
        };
    },
    methods: {
        getRandomLinks(count) {
            const links = [...this.footerLinks];
            const randomLinks = [];
            for (let i = 0; i < count; i++) {
                const randomIndex = Math.floor(Math.random() * links.length);
                randomLinks.push(links.splice(randomIndex, 1)[0]);
            }
            return randomLinks;
        },
    },
};
</script>

<template>
    <footer>
        <div class="container foot-flex">

            <div class="lists">
                <ul>
                    <h3 class="white-color">DC COMICS</h3>
                    <li v-for="link in getRandomLinks(7)" :key="link.text">{{ link.text }}</li>
                    <h3 class="white-color">SHOP</h3>
                    <li v-for="link in getRandomLinks(2)" :key="link.text">{{ link.text }}</li>
                </ul>

                <ul>
                    <h3 class="white-color">DC</h3>
                    <li v-for="link in getRandomLinks(7)" :key="link.text">{{ link.text }}</li>
                    <li v-for="link in getRandomLinks(5)" :key="link.text">{{ link.text }}</li>
                </ul>

                <ul>
                    <h3 class="white-color">SITES</h3>
                    <li v-for="link in getRandomLinks(5)" :key="link.text">{{ link.text }}</li>
                </ul>

            </div>

            <img class="bg-logo" src="../assets/img/dc-logo-bg.png" alt="logo-bg">

        </div>

        <!--LAST CONTAINER:-->
        <div class="social-link container">
            <button class="sign_button white-color">SIGN-UP NOW!</button>
            <div class="social-container">
                <h2 class="blue_color">FOLLOW US</h2>
                <img src="../assets/img/footer-facebook.png" alt="fb">
                <img src="../assets/img/footer-twitter.png" alt="tw">
                <img src="../assets/img/footer-youtube.png" alt="yt">
                <img src="../assets/img/footer-pinterest.png" alt="pnt">
                <img src="../assets/img/footer-periscope.png" alt="pos">
            </div>
        </div>

    </footer>
</template>

<style scoped>
footer {
    color: #6f787e;
    background-image: url(../assets/img/footer-bg.jpg);
}

.lists {
    display: flex;
    justify-content: flex-start;
    gap: 15px;
    line-height: 27px;
}


.foot-flex {
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: relative;
}

.foot-flex img {
    object-fit: contain;
}

.bg-logo {
    position: absolute;
    right: 5px;
}

.white-color {
    color: white;
}

.lists li:hover {
    cursor: pointer;
    color: white;
}

/*LAST CONTAINER:*/
.social-link {
    height: 80px;
    background-color: #303030;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    z-index: 1;
}

.blue_color {
    color: #047eee;
    text-align: start;
    margin-right: 20px;
}

.sign_button {
    background-color: #303030;
    border: solid #047eee 2px;
    padding: 15px 10px 15px 10px;
    margin-left: 40px;
}

.social-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
}

.social-container img {
    padding-left: 5px;
    padding-right: 5px;
    width: 40px;
    object-fit: contain;
}

.sign_button:hover {
    background-color: #047eee;
    cursor: pointer;
}
</style>