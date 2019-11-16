<script>
  const dictionaries = [
    {
      name: 'Universitet i Bergens Ordbok',
      description: 'The University of Bergen\'s dictionary.',
      href: 'https://ordbok.uib.no/',
      tags: {
        bokmål: true,
        nynorsk: true,
        english: false,
        examples: true,
        inflections: true,
      },
    },
    {
      name: 'Norske Akademis Ordbok',
      description: 'The Norwegian Academy\'s dictionary.',
      href: 'https://www.naob.no/ordbok/',
      tags: {
        bokmål: true,
        nynorsk: true,
        english: false,
        examples: true,
        inflections: true,
      },
    },
    {
      name: 'bab.la',
      description: 'bab.la\'s Norwegian-English dicationary.',
      href: 'https://en.bab.la/dictionary/norwegian-english/',
      tags: {
        bokmål: true,
        nynorsk: false,
        english: true,
        examples: true,
        inflections: false,
      },
    },
  ];
</script>

<h1 class="title">Dictionaries</h1>

{#each dictionaries as dict}
  <section class="section">
    <header>
      <h2 class="title is-4">{dict.name}</h2>
      <h3 class="subtitle is-5">
        <a href={dict.href}>{dict.href}</a>
      </h3>

      <div class="field is-grouped is-grouped-multiline">
        {#each Object.keys(dict.tags) as tag}
          <div class="control">
            <div class="tags has-addons">
              <span class="tag is-dark">{tag}</span>
              <span class="tag {dict.tags[tag] ? 'is-success' : 'is-danger'}">{dict.tags[tag]}</span>
            </div>
          </div>
        {/each}
      </div>
    </header>

    <p>{dict.description}</p>
  </section>
{/each}
