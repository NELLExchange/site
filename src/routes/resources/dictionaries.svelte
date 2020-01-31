<script>
  import TagList from '../../components/TagList.svelte';

  const dictionaries = [
    {
      name: 'Universitet i Bergens Ordbok',
      description: `<p>The University of Bergen's dictionary.</p><p>Contains the official writing standard and all allowed variants of Norwegian.</p>`,
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
      description: `<p>The Norwegian Academy's dictionary.</p><p>Contains a small sub-set of 'moderat' bokmål and riksmål (not official).</p><p>This makes this dictionary better at handling slang.</p>`,
      href: 'https://www.naob.no/ordbok/',
      tags: {
        bokmål: true,
        nynorsk: false,
        english: false,
        examples: true,
        inflections: true,
      },
    },
    {
      name: 'bab.la',
      description: `<p>bab.la's Norwegian-English dictionary.</p><p>If you need English translations of words, this site often does a better job than Google Translate.</p>`,
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

<section class="section">
  <div class="container is-fluid">
    <h1 class="title">Dictionaries</h1>

    {#each dictionaries as dict}
      <article class="message">
        <div class="message-header">
          <p>{dict.name}</p>
        </div>
        <div class="message-body">
          <TagList tags={dict.tags}/>

          <div class="content">
            {@html dict.description}

            <p><a href={dict.href}>{dict.href}</a></p>
          </div>
        </div>
      </article>
    {/each}
  </div>
</section>
