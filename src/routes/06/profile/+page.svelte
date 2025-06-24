Olá! 👋
Seja muito bem-vindo(a)!
<script>
    import { page } from '$app/stores';
    import { derived } from 'svelte/store';
    const email = derived(page, $page => $page.url.searchParams.get('email'));
  </script>
  
  <h1>Bem-vindo(a)!</h1>
  <p>{$email}</p>