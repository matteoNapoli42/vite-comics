<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>


<template>
    <div class="col-2 py-5">
        <img :src="thumb" style="height: 180px; width: 180px;">
        <h6 style="color: white;">{{ series }}</h6>
    </div>
</template>



<style></style>