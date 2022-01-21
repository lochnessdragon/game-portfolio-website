<script>
	import '../app.css';
</script>

<!-- header -->
<ul>
	<li><a href="/">Home</a></li>
	<li><a href="/about">About</a></li>
	<li><a href="/faq">FAQ</a></li>
	<li><a href="/presskit">Press Kit</a></li>
</ul>
<!-- /header -->

<slot />

<!-- footer -->
<div class="bg-slate-700 text-slate-100 py-9">
	<p class="text-center">
	© 2022 Copyright: <span class="font-medium">lochnessdragon</span>
	</p>
</div>
<!-- /footer -->