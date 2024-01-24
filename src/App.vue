<script>

    import AppHeader from './components/AppHeader.vue'
    import AppMain from './components/AppMain.vue'
    import AppFooter from './components/AppFooter.vue'
    import axios from 'axios';

export default {
    data() {
        return {
            store
        };
    },
    components: {
        AppHeader,
        AppMain,
        AppFooter
    },
    methods: {

        getResult () {
            axios
                
                .get(this.store.baseUrl,
                    params: {
                        
                    }
                )
        }
    }
    
}

</script>

<template>

    <AppHeader/>
    <AppMain/>
    <AppFooter/>

</template>

<style>

</style>
