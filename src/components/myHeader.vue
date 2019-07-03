<template>
<div class="hide-overflow" style="position: relative;">
    <v-toolbar fixed color="pink lighten-3">
      <v-btn flat icon to="/" color="white">
        <v-icon>home</v-icon>
      </v-btn>
      <v-toolbar-title class="white--text">YEONJI'S BLOG</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn to="/post" class="white--text" flat>Post</v-btn>
        <v-btn to="/portfolio" class="white--text" flat>Portfolio</v-btn>
        <v-btn to="/login" class="white--text" flat>Login</v-btn>
        <v-btn class="white--text" flat><a href="#" id="favorite" title="즐겨찾기 등록" style="color:white;text-decoration:none">
          <v-icon>star</v-icon></a>
        </v-btn>
      </v-toolbar-items>
      <v-toolbar-side-icon class="hidden-sm-and-up white--text" @click="drawer = !drawer"></v-toolbar-side-icon>
    </v-toolbar>

    <v-navigation-drawer app right disable-resize-watcher v-model="drawer" class="pink lighten-3">
      <v-list>
        <v-list-tile @click="$router.push('/post')">
          <v-list-tile-content>
            <v-list-tile-title class="white--text title">Post</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile @click="$router.push('/portfolio')">
          <v-list-tile-content>
            <v-list-tile-title class="white--text title">Portfolio</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile @click="$router.push('/login')">
          <v-list-tile-content>
            <v-list-tile-title class="white--text title">Login</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>

</div>
</template>

<script>
export default {
  name: 'myHeader',
  props: {},
  data(){
    return {
      drawer:false
    }
  }
}
</script>
