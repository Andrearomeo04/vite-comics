<script>
import { links_1 } from '../data/footer_links'
export default {
    data () {
        return {
            links_1
        }
    }
}
</script>

<template lang="">
    <div id="background">
        <div class="container text-white">
            <div class="row">
                <div class="col-2 d-flex flex-column">
                    <h2>DC COMICS</h2>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links_1" :key="index" class="my-3 text-secondary">
                            {{ link.text }}
                        </li>
                    </ul>
                    <h2>LOL</h2>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links" :key="index" class="my-3 text-secondary">
                            {{ link.text }}
                        </li>
                    </ul>
                </div>
                <div class="col-2 d-flex">
                    <h2>DC</h2>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links" :key="index" class="my-3 text-secondary">
                            {{ link.text }}
                        </li>
                    </ul>
                </div>
                <div class="col-2 d-flex">
                    <h2>SITES</h2>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links" :key="index" class="my-3 text-secondary">
                            {{ link.text }}
                        </li>
                    </ul>
                </div>

                <div class="col-6 d-flex">
                    <div class="logo-footer">
                        <img src="../assets/img/dc-logo-bg.png" alt="logo">
                    </div>
                </div>
            </div>
        </div> 
    </div>
    <div id="bg-gray">
        <div class="container">
            <div class="row">
                <div class="col-8 d-flex">
                    
                </div>
                <div class="col-4 d-flex">
                    
                </div>
            </div>
        </div> 
    </div>
    <div id="bg-black">
        <div class="container">
            <div class="row">
                <div class="col-8 d-flex">
                    
                </div>
                <div class="col-4 d-flex">
                    
                </div>
            </div>
        </div> 
    </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;

    #background {
        background-image: url(../assets/img/footer-bg.jpg);
    }
    
    .logo-footer {
        img {
            width: 400px;
            object-fit: contain;
            overflow: hidden;
        }
    }

    #bg-gray {
        background-color: $footer-color;
        height: 100px;
    }

    #bg-black {
        background-color: black;
        height: 80px;
    }
    
</style>