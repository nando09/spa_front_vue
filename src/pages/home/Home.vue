<template>
	<site>
		<publicar-conteudo/>
		<card-conteudo perfil="https://materializecss.com/images/yuna.jpg" nome="Maria 3 do Bairro" data="12-12-2019">
			<card-detalhe img="https://materializecss.com/images/sample-1.jpg" titulo="Testando" texto="I am a very simple card. I am good at containing small bits of information.
				I am convenient because I require little markup to use effectively."/>
		</card-conteudo>
	</site>
</template>

<script>
import Site from '@/templates/Site'
import CardConteudo from '@/components/social/CardConteudo'
import CardDetalhe from '@/components/social/CardDetalhe'
import PublicarConteudo from '@/components/social/PublicarConteudo'

export default {
	name: 'Home',
	components:{
		CardConteudo,
		CardDetalhe,
		PublicarConteudo,
		Site
	},
	data () {
	return {

	}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
