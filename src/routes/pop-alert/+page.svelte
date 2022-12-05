<script lang="ts">
  import svelteWelcome from "$lib/images/svelte-welcome.png"

  const attack = '" onload="alert(\'uhoh\')" data-nothing="not important'
</script>

<img src={svelteWelcome} style:--css-variable={attack} alt="dangerous attributes ssr">

<p>
  Did you see an alert popup?
</p>