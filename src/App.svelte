<script>
	import { Router, Route, Link } from "svelte-routing";
	import Basket from "./Basket.svelte";
	import Catalog from "./Catalog.svelte";
	import Profile from "./Profile.svelte";
	import Signin from "./Signin.svelte";
</script>

<main />
<Router>
	<Route path="/" component={Signin} />
	<Route path="/catalog" component={Catalog} />
	<Route path="/basket" component={Basket} />
	<Route path="/profile" component={Profile} />
</Router>

<style>
	main {
		padding: 0;
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
