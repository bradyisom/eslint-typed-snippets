<script lang="ts">
	function hello() {
		console.log('Hello');
	}
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

{@render editor_button({ onclick: hello })}

<!-- prettier-ignore -->
{#snippet editor_button(foo: {
    onclick: () => void,
})}
  <button on:click={foo.onclick}>Click me</button>
{/snippet}
