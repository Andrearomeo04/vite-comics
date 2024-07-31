<script>
export default {
    props: {
        thumb: string,
        series: string,
        price: string,
        type: string
    },
}

</script>

<template lang="">
    <div>
        <div class="container">
                <div class="row">
                    <div class="col-2 text-white py-5">
                        <div class="thumb">
                            <img :src="thumb">
                        </div>
                        <h6>{{ series }}</h6>
                        <h6>{{ price }}</h6>
                        <h6>{{ type }}</h6>
                    </div>
                </div>
            </div>
    </div>
</template>

<style lang="">
    
</style>