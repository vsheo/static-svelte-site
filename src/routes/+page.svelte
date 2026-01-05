<script>
  let { data } = $props();
</script>

<h1>Welcome to a SvelteKit static site</h1>
<p>
  Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
  documentation
</p>

<img
  src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXTFRwk4pvnHBw0bD7D-G5hr2PmiCEkxYuXw&s"
  alt="mekanik"
/>
<a href="/detailspage">details page</a>

<h2>Data van supabase</h2>
<ul>
  {#each data.instruments as instrument}
    <li>{instrument.name}</li>
  {/each}
</ul>
