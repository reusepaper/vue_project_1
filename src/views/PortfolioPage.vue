<template>
  <div>
    <myHeader></myHeader>
    <ImgBanner imgSrc="https://source.unsplash.com/random/1600x900">
      <div style="line-height:1.2em;font-size:1.2em;" slot="text">Portfolio</div>
    </ImgBanner>
    <v-container>

      <!-- Portfolio -->
      <v-layout>
        <v-flex xs12>
          <PortfolioList :limits="8" :load-more="true"></PortfolioList>
        </v-flex>
      </v-layout>

    </v-container>
    <myFooter></myFooter>
  </div>
</template>

<script>
import myHeader from '../components/myHeader'
import ImgBanner from '../components/ImgBanner'
import PortfolioList from '../components/PortfolioList'
import myFooter from '../components/myFooter'

export default {
	name: 'PortfolioPage',
	components: {
    myHeader,
		ImgBanner,
		PortfolioList,
    myFooter
	},
}
</script>
