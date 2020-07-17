<template>
	<div id="app">
		<header>
			<nav-bar logo="Social" url="#" cor="green darken-1"/>
		</header>
		<main>
			<div class="container">
				<div class="row">
					<grid-vue tamanho="6">
						<card-menu>

						</card-menu>
					</grid-vue>
					<grid-vue tamanho="6">
						<slot />
						<router-view/>
					</grid-vue>
				</div>
			</div>
		</main>
		<footer-vue cor="green darken-1" logo="Social" descricao="Teste descrição" ano="2020">
			<li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
		</footer-vue>
	</div>
</template>

<script>
import NavBar from '@/components/layouts/NavBar'
import FooterVue from '@/components/layouts/FooterVue'
import GridVue from '@/components/layouts/GridVue'
import CardMenu from '@/components/layouts/CardMenu'


export default {
	name: 'LoginTemplate',
	components:{
		NavBar,
		FooterVue,
		GridVue,
		CardMenu
	}
};
</script>

<style>

</style>
