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

<nav class="bg-gradient-to-t from-gray-50 to-gray-600">
	<div class="mx-auto px-8 py-1">
		<div class="flex justify-between">
			<!--Block Logo + primary nav-->
			<div class="flex space-x-4">
				<!--logo-->
				<div class="flex items-center py-1">
					<div class="h-9 w-9 sm:h-12 sm:w-12 bg-red-400 flex justify-center items-center">
						<h3 class="text-white text-xl sm:text-2xl font-extrabold">M</h3>
					</div>
					<div class="h-9 w-9 sm:h-12 sm:w-12 bg-red-400/50 flex justify-center items-center">
						<h3 class="text-white text-xl sm:text-2xl font-extrabold">Y</h3>
					</div>
					<div class="ml-3 text-xl  sm:text-xl font-bold">Studio's</div>
				</div>
				<!--fin logo-->

				<!--Primary nav
				<div class="hidden md:flex items-center space-x-2 text-xl font-bold">
					<a class="py-5 px-3 text-slate-200 hover:text-red-900 transition duration-300" href="/">Inicio</a>
					<a class="py-5 px-3 text-slate-200 hover:text-red-900 transition duration-300" href="/">Trabaja con nosotros</a>
				</div>
				<!--fin primary nav-->
			</div>
			<!--End block logo + primary nav-->

			<!--secundary nav-->
			<div class="hidden md:flex items-center space-x-2 sm:text-sm lg:text-xl">
				<a class="py-5 px-3  hover:text-slate-200 transition duration-300" href="/">Quienes somos</a>
				<a class="py-5 px-3  hover:text-slate-200 transition duration-300" href="/">Trabaja con nosotros</a>
				<a class="py-5 px-3  hover:text-slate-200 transition duration-300" href="/">Porcentaje</a>
					<a class="py-5 px-3 hover:text-slate-200 transition duration-300" href="/">Horarios</a>
				<!--a class="text-slate-200 py-5 px-5 hover:text-red-900 font-bold" href="/">Opciones</a>
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
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Quienes somos</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Trabaja con nosotros</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/">Porcentaje</a>
		<a on:click={buttonToggle} class="block py-1 px-3 text-sm hover:bg-blue-500" href="/" >Horario</a>
	</div>
</nav>