<script>
  const dictionaries = [
    {
      description: 'Some description.',
      href: 'https://ordbok.uib.no/',
      name: 'Some Name',
    },
    {
      description: 'Some description 2.',
      href: 'https://ordbok.uib.no/',
      name: 'Some Name 2',
    },
  ];
</script>


<div class="container">
  <h1 class="title">Dictionaries</h1>

  {#each dictionaries as dict}
    <section class="section">
      <div class="container">
        <h1 class="title">{dict.name}</h1>
        <h2 class="subtitle">
          <a href={dict.href}>{dict.href}</a>
        </h2>
        <p>{dict.description}</p>
      </div>
    </section>
  {/each}
</div>
