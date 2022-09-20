<script>
	import '../app.css';
	import logo from '../logos.svg'
	import Navbar from '../components/Navbar.svelte';
</script>

<div class="sticky top-0 z-20">
	<Navbar />
</div>

<div class="fixed w-screen flex h-screen justify-center -z-10">
	<img src={logo} alt="">
</div>

<slot />


