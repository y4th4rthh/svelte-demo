<script>
 import { goto } from '$app/navigation';
    let userId='';
    const handleClick = () =>{
       goto(`/user/${userId}`)
    }
    const handleTextChange = (e) =>{
        userId = e.target.value
    }
</script>

<h1 class="text-center">Welcome to SvelteKit</h1>
<input type="text" on:input={handleTextChange}/>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<button on:click={handleClick}>Navigate</button>
