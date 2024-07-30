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
                    <div v-for="(icon, index) in icons" :key="index">
                        <img :src="icon.img" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="">
    
</style>