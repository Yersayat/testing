<template>
<div class="v-main-wrapper2">
    <h1>{{ name }}</h1>
</div>
</template>

<script>
export default{
    name: 'v-main-wawrpper2',
    components: {
        
    },

    data() {
        return {
            name: 'Aidos'
        }
    },
    computed: {},
    methods: {},
    watch: {}

}
</script>

<style>
.v-main-wrapper2 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 900px;
    margin: 0 auto;
}
</style>