<template>
  <div class="hide-overflow" style="position: relative;">
    <v-toolbar fixed color="teal">
      <v-toolbar-title class="white--text">YEONJI'S BLOG</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn class="white--text" flat>Post</v-btn>
        <v-btn class="white--text" flat>Portfolio</v-btn>
        <v-btn class="white--text" flat>Login</v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </div>
</template>

<script>

export default {
	name: 'myHeader',
	props: {
		text: {type: String}
	},
	methods: {
	},
}
</script>
