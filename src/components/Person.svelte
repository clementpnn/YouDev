<script>
  // export let state

  let person = [
		{ name: 'DevTheory', stack: 'Front End', lang: 'FR' },
		{ name: 'Neolectron', stack: 'Front End', lang: 'FR' },
		{ name: 'Stéphane - smo', stack: 'Front End', lang: 'FR' },
		{ name: 'Benjamin Code', stack: 'Front End', lang: 'FR' },
		{ name: 'Melvin', stack: 'Front End', lang: 'FR' },
		{ name: 'ThePrimeagen', stack: 'Front End', lang: 'EN' },
		{ name: 'Theo ping.gg', stack: 'Front End', lang: 'EN' },
		{ name: 'Grafikart', stack: 'Full Stack', lang: 'FR' },
		{ name: 'Le Designer du Web', stack: 'Front End', lang: 'FR' },
		{ name: 'Fireship', stack: 'Full Stack', lang: 'FR' },
		{ name: 'William Candillon', stack: 'Mobile', lang: 'EN' },
	]
</script>

{#each person as { name, stack, lang }, id}
  <div class='container'>
    <span class='name'>{name}</span>
    <span class='stack'>{stack}</span>
    <span class='lang'>{lang}</span>
    <!-- <span>{id + 1}</span> -->
    <!-- <span>{state}</span> -->
  </div>
{/each}

<style>
  .container {
    height: 6rem; /* 96px */
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    font-family: var(--font);
    background-color: #FBF9F9;
    border-top: 1px solid #000;
    border-left: 1px solid #000;
    border-right: 1px solid #000;
  }

  .container:last-child {
    border-bottom: 1px solid #000;
  }

  .container:hover {
    background-color: var(--cta);
  }

  .name {
    font-size: 1.225rem;
    margin-bottom: 0.5rem; /* 8px */
  }

  .stack {
    font-size: 1rem;
  }

  .lang {
    font-size: 1rem;
    position: absolute;
    right: 16px;
    top: 50%;
    transform: translateY(-50%);
    padding: 6px 16px;
    border: 1px solid #000;
    border-radius: 100%;
  }

</style>