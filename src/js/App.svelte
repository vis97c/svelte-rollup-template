<script>
	import '../scss/main.scss'
	import { Router } from 'svelte-router-spa'
	import { routes } from './views'

	export let name;
</script>
<style type="text/scss">
	@import '../scss/base/svelte.scss';
	$color: red;
	h1 {
		color: $color;
		@include flexbox(column, nowrap, flex-start, stretch);
		// display: none;
	}
	/* main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	} */
</style>

<h1>Hello {name}!</h1>
<Router {routes} />