<script>
import { icons } from '../data/icons'
export default {
    data () {
            return {
                icons
            }
         } 
}
</script>

<template lang="">
    <div class="bg-black">
        <div class="container">
            <div class="row">
                <div class="col-12 text-white py-5">
                    <h4>Content goes here</h4>
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
                        <p class="ms-5 mb-0">{{ icon.text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    .inside {
        img {
            width: 50px;
        }
    }
</style>