<script>
export default {
    data() {
        return {
            headerNavVoices:
                [
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Games",
                    "Collectibles",
                    "Videos",
                    "Fans",
                    "News",
                    "Show"
                ]
        };
    },
};



</script>

<template>
    <header class="d-flex justify-content-between container">
        <div class="col-6 py-3">
            <img src=".././assets/img/dc-logo.png" alt="" style="height: 86px;">
        </div>
        <div class="col-6 py-4">
            <nav class="navbar navbar-expand justify-content-center">
                <ul class="nav navbar-nav" v-for="elem in headerNavVoices">
                    <a href="" class="nav-item nav-link">{{ elem }}</a>
                </ul>
            </nav>
        </div>

    </header>
</template>

<style scoped>
ul {
    list-style: none;
}

a {
    text-decoration: none;
    color: black;
}

/*a::after {
    content: "";
    height: 5px;
    position: absolute;
    background-color: blue;
    width: 5%;
    bottom: 85.7%;
    bottom: 0;
}

li:hover::after {}
*/
</style>