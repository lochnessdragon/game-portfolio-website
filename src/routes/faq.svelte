
<script>
	import QuestionAnswer from "$lib/components/question-answer.svelte";

	const questions = [
		{
			"question": "What is the price of this game?",
			"answer": "$4.99"
		},
		{
			"question": "What platforms does this game run on?",
			"answer" : "Windows, Linux, Macos, Xbox, Nitendo Switch and Playstation!"
		}
	]
</script>

<h1>Frequently Asked Questions</h1>

{#each questions as question}
	<QuestionAnswer question={question.question} answer={question.answer} />
{/each}