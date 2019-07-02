<template>
  <div class="hide-overflow" style="position: relative;">
    <v-toolbar fixed color="teal">
      <v-toolbar-title class="white--text">YEONJI'S BLOG</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn v-for="link in links" :key="link.text" :to="link.page" class="white--text" flat>{{link.text}}</v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </div>
</template>

<script>

export default {
	name: 'myHeader',
	props: {
	},
  data: () => ({
    links: [
      {text:'Home', page:'/'},
      {text:'Post', page:'/post'},
      {text:'Portfolio', page:'/portfolio'},
      {text:'Login', page:'/login'}
    ]
  })
}
</script>
