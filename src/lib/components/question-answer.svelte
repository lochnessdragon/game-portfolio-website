<script>
	export let question = "";
	export let answer = "";

	let expanded = false;
</script>

<div class="bg-orange-800 text-white font-serif">
	<button class="bg-orange-900 w-full text-left p-2.5" on:click={() => expanded = !expanded}>
		<h1 class="text-3xl">Q: {question}</h1>
	</button>
	<p hidden={!expanded} class="text-lg p-2.5 transition-all">A: {answer}</p>
</div>