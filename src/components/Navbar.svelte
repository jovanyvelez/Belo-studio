<script>
	import src from '../logo.png'
	let buttonMenu = true;
	let showClass = 'hidden';
	let margin = 0;
	const buttonToggle = () => {
		buttonMenu = !buttonMenu;
		buttonMenu ? (showClass = 'hidden') : (showClass = '');
	};

</script>


<!--********************Inicia la interfaz-->

<nav class="bg-gradient-to-t from-gray-50 to-gray-800">
	<div class="mx-auto px-8">
		<div class="flex justify-between">
			<!--Block Logo + primary nav-->
			<div class="flex space-x-4">
				<!--logo-->
				<div>
					<a class="flex items-center py-5 px-3 text-red-800 hover:text-blue-600" href="/">
						<img {src} class="mr-3 h-36 w-36" alt="Logo" />
					</a>
				</div>
				<!--fin logo-->

				<!--Primary nav-->
				<div class="hidden md:flex items-center space-x-2 text-xl font-bold">
					<a class="py-5 px-3 text-slate-200 hover:text-red-900 transition duration-300" href="/">Inicio</a>
					<a class="py-5 px-3 text-slate-200 hover:text-red-900 transition duration-300" href="/">Trabaja con nosotros</a>
				</div>
				<!--fin primary nav-->
			</div>
			<!--End block logo + primary nav-->

			<!--secundary nav-->
			<div class="hidden md:flex items-center space-x-2 text-xl">
				<a class="text-slate-200 py-5 px-5 hover:text-red-900 font-bold" href="/">Opciones</a>
				<!--a class="py-2 px-3 bg-blue-600 text- rounded hover:bg-violet-500 hover:text-black transition duration-300" href="https://engine.lobbypms.com/botanico-hotel-boutique" target="_blank">Reservas</a-->
			</div>

			<!--Mobile button goes here-->
			<div class="md:hidden flex items-center">
				<button on:click={buttonToggle}>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-6 w-6"
						viewBox="0 0 20 20"
						fill="currentColor"
					>
						<path
							fill-rule="evenodd"
							d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
							clip-rule="evenodd"
						/>
					</svg>
				</button>
			</div>
		</div>
	</div>
	<div class=" {showClass} md:hidden text-xl font-bold">
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Inicio</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Nosotros</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Trabaja con nosotros</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/" >Galeria</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Otros</a>
	</div>
</nav>