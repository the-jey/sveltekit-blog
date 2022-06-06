<script>
	export let pages;
</script>

<div class="navbar bg-base-100">
	<div class="flex-1">
		<a class="btn btn-ghost normal-case text-xl">Jey Blog</a>
	</div>
	<div class="flex-none">
		<ul class="menu menu-horizontal p-0">
			<li><a href="/">Home</a></li>
			{#each pages as { title, slug }}
				<li><a href={`/${slug}`}>{title}</a></li>
			{/each}
		</ul>
	</div>
</div>
