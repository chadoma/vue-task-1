<template>
    <div id="home">
        <v-app-bar
            color="rgba(100, 130, 183, 0.6)"
            dark
            flat
        >
            <NavItems/>
        </v-app-bar>
<HeroItems/>
    </div>
</template>

<script>
import HeroItems from '@/components/HeroItems'
import NavItems from '@/components/NavItems'
export default {
    name: 'Home',
    components:{
        NavItems,
        HeroItems
    }
};
</script>

