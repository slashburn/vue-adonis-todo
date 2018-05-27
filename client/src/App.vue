<template>
    <v-app>
        <v-toolbar color="green" dark fixed>
            <v-toolbar-title class="mr-4">VUE TODO</v-toolbar-title>
            <v-toolbar-items>
                <v-btn flat>
                    <v-icon>playlist_add_check</v-icon>
                    Projects
                </v-btn>
            </v-toolbar-items>
            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-sm-and-down">
                <v-btn flat><v-icon>account_box</v-icon>Register</v-btn>
                <v-btn flat><v-icon>fingerprint</v-icon>Login</v-btn>
                <v-btn flat><v-icon>exit_to_app</v-icon>Logout</v-btn>
                <v-btn flat><v-icon>ondemand_video</v-icon>How this was Made</v-btn>
            </v-toolbar-items>
        </v-toolbar>
        <div id="app">
            <div id="nav">
                <router-link to="/">Home</router-link>
                |
                <router-link to="/about">About</router-link>
            </div>
            <router-view/>
        </div>
    </v-app>
</template>

<style lang="scss">
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }

    #nav {
        padding: 30px;
        a {
            font-weight: bold;
            color: #2c3e50;
            &.router-link-exact-active {
                color: #42b983;
            }
        }
    }
</style>
