<script>
	import About from "./components/About.svelte";
	import Text from "./components/Text.svelte";
	import Person from "./components/Person.svelte";

	export let name;
	export let lastName;
	
	//Objeto a transmitir en este componente

	const data = {
		name: "Juan",
		lastName: "Esteban",
		age: 22,
	};
</script>

<main>
	<h1>Hello {name} {lastName}!</h1>
	<About />
	<Text anotherText="Hola, soy el texto de props con another Text" />
	<Text />
	<Person {...data} />
	<!-- Person name={data.name} lastName={data.lastName} age={data.age} /-->
	<!-- Person {name} {lastName} {age}/-->
	
</main>

<style>
	:global(body) {
		background-color: #f2eee2;
		color: #0084f6;
	}
	:global(body.dark-mode) {
		background-color: black;
		color: white;
	}
	:global(:root) {
		--theme-color: purple;
	}

	

	main {
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
	}
</style>
