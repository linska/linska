<template>
    <v-app-bar
            app
            color="white"
            flat
            light
            style="padding: 1rem 15% 0 15%;"
    >

        <div class="d-flex">
            <v-img
                    alt="Logo"
                    class="shrink"
                    contain
                    src="../src/assets/logo.png"
                    transition="scale-transition"
            />
        </div>
        <v-spacer></v-spacer>
        <v-toolbar-items id="appbar" >
            <v-btn
                    id="btnbar"
                    v-for="item in barbtn" :key="item.title"
                    color="transparent"
                    class="text-none primary--text"
                    style=" font-family: 'Roboto', sans-serif;
                                font-weight: normal;
                                letter-spacing: normal;
                                font-size: 18px;
                                padding: 0 13px 0 13px"
                    depressed>
                {{ item.title}}
            </v-btn>
        </v-toolbar-items>

    </v-app-bar>
</template>

<script>
    export default {
        name: "AppBar",
        computed:{
            barbtn () {
                return [
                    {title: 'Обо мне'},
                    {title: 'Консультации'},
                    {title: 'Мои проекты'},
                    {title: 'Книги'},
                    {title: 'Халява, плиз!'},
                    {title: 'Контакты'}
                ]
            },
        }
    }
</script>

<style scoped>

</style>