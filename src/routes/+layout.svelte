<script lang="ts">
	import { base } from '$app/paths';
	import Contacts from '$lib/Contacts.svelte';
</script>

<header>
	<h1>Mosab "IVIosab" Mohamed</h1>
	<nav>
		<ul>
			<li><a href="{base}/">Home</a></li>
			<li><a href="{base}/about">About</a></li>
			<li><a href="{base}/projects">Projects</a></li>
			<li><a href="{base}/comic">Comic</a></li>
		</ul>
	</nav>
</header>
<main>
	<slot />
</main>
<footer>
	<p>&copy; Mosab Mohamed 2023</p>
	<Contacts />
</footer>

<style>
	footer {
		box-sizing: border-box;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 1rem;
		background-color: #333;
		color: #fff;
		position: fixed;
		left: 0;
		bottom: 0;
		width: 100%;
	}
	p {
		margin: 5px;
	}
	header {
		box-sizing: border-box;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem;
		background-color: #333;
		color: #fff;
	}
	nav ul {
		display: flex;
		list-style: none;
	}

	nav ul li {
		margin: 0 1rem;
	}

	nav a {
		color: #fff;
	}

	a {
		text-decoration: none;
		color: black;
	}
	main {
		padding-top: 5rem;
	}
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
</style>
