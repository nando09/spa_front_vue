<template>
	<div class="row">
		<grid-vue class="input-field" tamanho="12">
			<textarea v-model="conteudo" class="materialize-textarea"></textarea>
			<label>Textarea</label>
		</grid-vue>
		<p>
			<grid-vue v-if="conteudo" class="btn waves-effect waves-light col s2 offset-s10" tamanho="2 offset-s10">Publicar</grid-vue>
		</p>
	</div>
</template>

<script>
import GridVue from '@/components/layouts/GridVue'

export default {
	name: 'PublicarConteudo',
	components:{
		GridVue
	},
	props: [],
	data () {
	return {
		conteudo: ''
	}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
