<template>
	<div id="app">
		<header>
			<nav-bar logo="Social" url="#" cor="green darken-1"/>
		</header>
		<main>
			<div class="container">
				<div class="row">
					<grid-vue tamanho="4">
						<card-menu>
							<div class="row valign-wrapper">
								<grid-vue tamanho="4">
									<img src="https://materializecss.com/images/yuna.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
								</grid-vue>
								<grid-vue tamanho="8">
									<span class="black-text">
										<h4>Maria do Bairro</h4>
										 Add the "circle" class to it to make it appear circular.
									</span>
								</grid-vue>
							</div>
						</card-menu>
						<card-menu>
							<h3>Teste</h3>
						</card-menu>
					</grid-vue>
					<grid-vue tamanho="8">
						<slot />
						<router-view/>
					</grid-vue>
				</div>
			</div>
		</main>
		<footer-vue cor="green darken-1" logo="Social" descricao="Teste descrição" ano="2020">
			<li><a class="grey-text text-lighten-3" href="#!">Login</a></li>
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
	name: 'Site',
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
