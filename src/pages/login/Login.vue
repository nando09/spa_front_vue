<template>
	<span>
		<login-template>
			<h2>Login</h2>
			<input type="text" name="name">
			<input type="password" name="senha">
			<button type="button" class="btn">Entrar</button>
		</login-template>
	</span>
</template>

<script>
import LoginTemplate from '@/templates/LoginTemplate'
import CardDetalhe from '@/components/social/CardDetalhe'
import PublicarConteudo from '@/components/social/PublicarConteudo'

export default {
	name: 'Login',
	components:{
		CardDetalhe,
		PublicarConteudo,
		LoginTemplate
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
