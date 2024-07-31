<script>
import { mainMenu } from '../data/menues'
export default {
         data () {
            return {
                mainMenu,
                activeIndex: 0,
            }
         },
         methods: {
            setActive (index) {
                this.activeIndex = index
            }
         }
}
</script>

<template lang="">
    <div class="bg-white position-fixed w-100 top-0 z-3">
        <div class="container">
            <div class="row">
                <div class="col-5 d-flex align-items-center">
                    <div class="">
                        <img src="../assets/img/dc-logo.png" alt="logo">
                    </div>
                </div>
                <div class="col-7 d-flex align-items-center">
                        <ul class="list-unstyled d-flex mb-0">
                            <li v-for="(items, index) in mainMenu" :key="index" class="mx-3" :class="index === activeIndex ? 'active' : ''" @click="setActive(index)">
                                {{ items.text }}
                            </li>
                        </ul>
                </div>
            </div>
        </div> 
    </div>
</template>
<style scoped lang="scss">
    @use '../styles/partials/variables' as *;

    ul {
        li {
            font-size: $font-1;
            cursor: pointer;
            padding: $padding-1 0px;
        }
    }
    .active {
        border-bottom: $active;
    }

</style>