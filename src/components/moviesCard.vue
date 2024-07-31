<script>
export default {
    props: {
        thumb: String,
        series: String,
        price: String,
        type: String
    },
}

</script>

<template lang="">    
    <div class="col-2 text-white py-5">
        <div class="thumb">
            <img :src="thumb" class="w-100 cards-height">
        </div>
        <h6>{{ series }}</h6>
        <h6>{{ price }}</h6>
        <h6>{{ type }}</h6>
    </div>
</template>

<style lang="scss">
.cards-height {
    max-height: 200px;
}
img {
    object-fit: cover;
    object-position: top;
}
</style>