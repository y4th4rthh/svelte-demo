<script>
  import { page } from '$app/stores';
  import { onMount } from 'svelte';

  let userId = '';

  $: userId = $page.params.userId;

  // or use onMount
  onMount(() => {
    console.log("User ID:", userId);
  });
</script>

<h1>Hello User {userId}</h1>
