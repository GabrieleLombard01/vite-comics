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
}

.card {
    flex-basis: 15%;
    padding: 20px;
}

.card img {
    display: block;
    width: 300px;
}

/*...*/
</style>