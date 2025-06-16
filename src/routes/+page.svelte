<script>
 import { goto } from '$app/navigation';
    const handleClick = () =>{
       goto('/about')
    }
</script>

<h1 class="text-center">Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<button on:click={handleClick}>Navigate</button>
