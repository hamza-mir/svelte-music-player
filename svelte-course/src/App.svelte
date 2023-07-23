<script>
	let name = "Svelte";
	let src = "https://picsum.com/200/200";
	let string = "Some <strong>string</strong> with html.";
</script>

<img {src} alt={name} />

<h1>
	Hello {name.toUpperCase()}
</h1>
<p>{@html string}</p>

<style>
	h1 {
		color: aquamarine;
	}
</style>
