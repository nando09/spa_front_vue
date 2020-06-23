<template>
	<div>
		<div v-if="img" class="card-image">
			<img :src="img">
			<span class="card-title">{{ titulo || ''}}</span>
		</div>
		<div v-if="texto" class="card-content">
			<p>{{texto}}</p>
		</div>
	</div>
</template>

<script>

export default {
	name: 'CardDetalhe',
	props: ['img', 'titulo', 'texto'],
	data () {
		return {

		}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
