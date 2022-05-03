<script>
	let count = 0;
	$: doubled = count * 2;

	function handleClick() {
		count += 1;
	}
</script>

<div class="container mx-auto border-2" style="max-width: 48rem;">
	<button on:click="{handleClick}" class="bg-blue-500 text-white p-4 rounded-md font-semibold">
		Clicked {count}
		{count === 1 ? 'time' : 'times'}
	</button>
	<p>{count} doubled is {doubled}</p>
</div>
