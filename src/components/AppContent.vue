<script>
import { icons } from '../data/icons'
import moviesCard from './moviesCard.vue'
export default {
    components: {
        moviesCard
    },
    data () {
            return {
                icons
            }
         } 
}
</script>

<template lang="">
    <div class="content">
        <div class="jumbo">
            <img src="../assets/img/jumbotron.jpg">
        </div>
        <div class="bg-black position-relative">
            <div class="container">
                <div class="row">
                    <div class="col-12 text-white py-5">
                        <span class="bg-primary py-3 px-4 fw-bold fs-3 blue-series">
                            CURRENT SERIES
                        </span>
                    </div>
                </div>
            </div>
            
        </div>
        <div class="bg-primary">
            <div class="container">
                <div class="row">
                    <div class="col-12 text-white py-5 d-flex justify-content-around">
                        <div v-for="(icon, index) in icons" :key="index" class="d-flex align-items-center inside">
                            <img :src="icon.img" />
                            <a href="#" class="ms-5 mb-0 text-white text-decoration-none">{{ icon.text }}</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    .content {
        margin-top: 130px;
    }

    .inside {
        img {
            width: 50px;
        }
    }
    .jumbo {
        img {
            object-fit: cover;
            object-position: top;
            width: 100%;
            height:400px;
        }
    }

    .blue-series {
        position: absolute;
        top: -35px;
    }
</style>