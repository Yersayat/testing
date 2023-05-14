<template>
    <div class="v-main-wrapper">
<p>{{ title }}</p>
<v-catalog />
<v-cart />

    </div>
</template>

<script>
import vCatalog from './v-catalog.vue'
import vCart from './v-cart.vue'

export default {
    name: 'v-main-wrapper',
    components: {
        vCatalog,
        vCart,
    },
    props: {},
    data() {
        return{
            title: 'Main wrapeer'
        }
    },
    computed: {}, //вычисление с компонентов
    methods: {}, //clicks, run animation, modal window
    watch: {}, //следить за изменениями чего либо и делать
    mounted() {
        console.log('Hello I am Iron Man')
    }

}
</script>

<style>
.v-main-wrapper {
    
    max-width: 900px;
    margin: 0 auto;
}
</style>