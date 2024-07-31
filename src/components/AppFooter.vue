<script>
import { links_1 } from '../data/footer_links'
import { links_2 } from '../data/footer_links'
import { links_3 } from '../data/footer_links'
import { links_4 } from '../data/footer_links'
import {socialIcons} from '../data/footer_links'
export default {
    data () {
        return {
            links_1,
            links_2,
            links_3,
            links_4,
            socialIcons
        }
    }
}
</script>

<template lang="">
    <div id="background">
        <div class="container text-white position-relative">
            <div class="row py-5">
                <div class="col-1 d-flex flex-column">
                    <h6>DC COMICS</h6>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links_1" :key="index" class="my-2">
                            <a href="#" class="text-decoration-none">{{ link.text }}</a>
                        </li>
                    </ul>
                    <h6>SHOP</h6>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links_2" :key="index" class="my-2">
                            <a href="#" class="text-decoration-none">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-1 d-flex flex-column">
                    <h6>DC</h6>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links_3" :key="index" class="my-2">
                            <a href="#" class="text-decoration-none">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-4 d-flex flex-column">
                    <h6>SITES</h6>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in links_4" :key="index" class="my-2">
                            <a href="#" class=" text-decoration-none">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>

                <div class="col-6 d-flex">
                    <div class="logo-footer">
                        <img src="../assets/img/dc-logo-bg.png" alt="logo" class="position-absolute">
                    </div>
                </div>
            </div>
        </div> 
    </div>
    <div id="bg-gray">
        <div class="container">
            <div class="row">
                <div class="col-8 d-flex text-white py-3">
                    <div class="sign-up p-3">
                        <h4 class="mb-0">SIGN-UP NOW!</h4>
                    </div>
                </div>
                <div class="col-4 d-flex align-items-center socials">
                    <h3>FOLLOW US</h3>
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
        overflow-y: hidden;
    }
    
    .logo-footer {
        img {
            width: 700px;
            object-fit: contain;
            top: -120px;
            right: -50px;
        }
    }

    .col-1,
    .col-4 {
        ul {
            li {
                font-size: 12px;
                a {
                    color: $footer-color;
                }
            }
        }
    }
    .col-1,
    .col-4 {
        ul {
            li {
                a:hover {
                    color: white;
                }
            }
        }
    }

    #bg-gray {
        background-color: $footer-color;
    }

    #bg-black {
        background-color: black;
        height: 80px;
    }

    .sign-up {
        border: $border_1;
        h4{
            font-size: $font_1;
        }
    }

    .socials {
        h3 {
            color: $color_1
        }
    }
    
</style>