<script context="module">
	/** @type {import('@sveltejs/kit').ErrorLoad} */
	export function load({ error, status }) {
		return {
			props: {
                error_code: `${status}`,
                error_message: `${error.message}`
			}
		};
	}
</script>

<script>
    export let error_code;
    export let error_message;

		const comments = [
            "I think you've explored a bit too far...",
            "Houston.... We have a problem!",
            "We're very sorry for the inconvenice. Some intern is going to be fired.",
            "🐒",
            "We rolled a nat 1...",
            "Alex, did you let Jerry into the server room again?",
            "Website 100",
            "Red pill or Blue pill?",
            "You sunk my Battleship!",
            "Looks like a creeper got into the server room again...",
            "$%#$%&#$%#%$#%#$#%$# technology",
            "This is why you NEVER mess with Tiamat.",
            "Knock knock. Who's there? Error 404: Joke Not Found",
            "Indiana Jones and the search for the missing web page.",
            "At least this is better than Jar Jar..."
        ];

    let comment = comments[Math.floor(Math.random() * comments.length)];
</script>

<svelte:head>
    <title>{error_code}: {error_message}</title>
</svelte:head>

<div class="text-center py-40">
    <h1 class="text-9xl font-black text-blue-600">{error_code}</h1>
    <p class="text-red-600">{error_message}</p><br/>
    
		<!-- Sarcastic Comment -->
		<p class="text-red-600">{comment}</p><br/>

    <a href="/" class="bg-blue-600 text-white rounded-3xl p-2.5 text-lg hover:p-3.5 hover:text-xl hover:bg-orange-600 transition-all"><button>Go home →</button></a>
</div>