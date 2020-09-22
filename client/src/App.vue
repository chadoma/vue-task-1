<template>
    <v-app>

        <div class="header">

            <router-view></router-view>
            <v-main>
            </v-main>
        </div>
    </v-app>
</template>

<script>

export default {
    name: 'App',

    data: () => ({
        //
    })
};
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Lato", sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    color: #777;
    padding: 10px;
}

.header {
    height: 99vh;
    background-image:
    linear-gradient(to right, rgba(0, 82, 212, .9), rgba(23, 175, 245, .9)),
    url("assets/solen-feyissa-jGmBZypoFPc-unsplash.jpg");
    background-size: cover;
    background-position: top;
  ;
}

</style>
