<script>
export default {
    data() {
        return {
            footerVoices: [
                {
                    title: "DC COMICS",
                    groupVoices: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },

                {
                    title: "SHOP",
                    groupVoices: [
                        "Shop DC",
                        "Shop DC Collectibles",
                    ]
                },

                {
                    title: "DC",
                    groupVoices: [
                        "Terms of Use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs"
                    ]
                },

                {
                    title: "SITES",
                    groupVoices: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa"
                    ]
                }
            ]
        }
    }

}
</script>

<template>
    <!--UpperFooter-->
    <section class="px-0" id="upperFooter">
        <div class="d-flex container">
            <div class="col-6 d-flex gap-0 py-5">
                <div class="col-3" v-for="(elem, index) in footerVoices">
                    <h5>{{ elem.title }}</h5>
                    <ul>
                        <li v-for="voice in footerVoices[index].groupVoices"><a href="">{{ voice }}</a></li>
                    </ul>
                </div>
            </div>
            <div class="col-6" id="bigLogo">

            </div>
        </div>
    </section>
    <!--LowerFooter-->
    <section id="lowerFooter">
        <div class="container d-flex py-4">
            <div class=" col-6">
                <button class="btn btn-outline-primary text-white">
                    SING-UP NOW!
                </button>
            </div>
            <div class="col-6 d-flex justify-content-end gap-3 align-items-center">
                <h5 style="color: #0481f9ff ;">FOLLOW US</h5>
                <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
            </div>
        </div>
    </section>
</template>

<style scoped>
#upperFooter {
    background: url("../assets/img/footer-bg.jpg");
    background-size: contain;
}

#lowerFooter {
    background-color: #303030ff;
}

h5 {
    color: white;
}

ul {
    list-style: none;
    padding-left: 0;
}

a {
    text-decoration: none;
    color: grey;
}

#bigLogo {
    background: url("../assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: right;
}
</style>