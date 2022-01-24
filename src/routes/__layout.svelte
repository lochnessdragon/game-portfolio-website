<script>
	import '../app.css';
	import Navbar from '$lib/components/navbar.svelte'
</script>

<!-- header -->
<Navbar />
<!-- /header -->

<slot />

<!-- footer -->
<div class="bg-slate-700 text-slate-100 py-9">
	<p class="text-center">
	© 2022 Copyright: <span class="font-medium">lochnessdragon</span>
	</p>
</div>
<!-- /footer -->