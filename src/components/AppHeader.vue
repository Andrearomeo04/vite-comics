<script>
import { mainMenu } from '../data/menues'
export default {
         data () {
            return {
                mainMenu
            }
         } 
}
</script>

<template lang="">
    <div>
        <div class="container">
            <div class="row">
                <div class="col-5 d-flex align-items-center py-4">
                    <div class="">
                        <img src="../assets/img/dc-logo.png" alt="logo">
                    </div>
                </div>
                <div class="col-7 d-flex align-items-center">
                        <ul class="list-unstyled d-flex mb-0">
                            <li v-for="(items, index) in mainMenu" :key="index" class="mx-3">
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
        }
    }

</style>