<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    },
}
</script>

<template>
    <section id="jumbotron">
    </section>

    <section id="series">
        <div class="container">
            <h1>{{ price }}</h1>
        </div>
    </section>
</template>

<style scoped>
#jumbotron {
    background-image: url("../assets/img/jumbotron.jpg");
    height: 408px;
}

#series {
    background-color: black;
}

h1 {
    color: white;
    margin: 0;
}
</style>