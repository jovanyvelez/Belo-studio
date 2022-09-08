<script>
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';
	import logo from '../logo.png'
</script>

<div class="sticky top-0 z-20">
	<Navbar />
</div>

<div>
	<img class="fixed -z-10 left-0 right-0 top-0 bottom-0 mx-auto h-screen" src={logo} alt="">
</div>

<slot />


