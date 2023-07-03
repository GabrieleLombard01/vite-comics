<script>
export default {
    props: {
        products: Array
    }
};
</script>

<template>
    <div class="content">
        <div class="container card-container">
            <div v-for="card in products" :key="card.series" class="card">
                <img :src="card.thumb" :alt="card.series">
                <h3>{{ card.series }}</h3>
            </div>

        </div>
    </div>
</template>

<style scoped>
.content {
    min-height: 90px;
    background-color: #1c1c1c;
    padding-top: 20px;
}

.card-container {
    display: flex;
    flex-wrap: wrap;
    margin-top: 2rem;
    padding-bottom: 4rem;
}

.card {
    flex-basis: calc(100% / 6);
    padding: 20px;
    margin-bottom: 30px;
}

.card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.card:hover {
    background-color: rgba(255, 255, 255, 0.423);
    cursor: pointer;
}

/*...*/
</style>