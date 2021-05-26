<template>
  <div id="app">
	<div>
		<h2>Laptop</h2>
		<a :href="'https://picsum.photos/id/' + n + '/800/600'" v-lightbox v-for="n in 9">
			<img :src="'https://picsum.photos/id/' + n + '/150/150'" alt="" />
		</a>
		<h2>Other</h2>
		<a :href="'https://picsum.photos/id/11' + n + '/800/600'" v-lightbox="'other'" v-for="n in 9">
			<img :src="'https://picsum.photos/id/11' + n + '/150/150'" alt="" />
		</a>
	</div>	
    <lightbox></lightbox>
  </div>
</template>
<script>
import Lightbox from "./components/lightbox/Lightbox";
export default {
  name: "App",
  components: {
    Lightbox
  }
};
</script>
<style>
	h2{
		font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
	}
</style>
