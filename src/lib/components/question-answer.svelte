<script>
	export let question = "";
	export let answer = "";

	let expanded = false;
</script>

<button on:click={() => expanded = !expanded}>
	<h1>Q: {question}</h1>
</button>
<p hidden={!expanded}>A: {answer}</p>