<script>
  import TagList from '../../components/TagList.svelte';

  const sites = [
    {
      name: 'grammatikk.com',
      description: `<p>Short Norwegian grammar cheat-sheets.</p>`,
      href: 'http://grammatikk.com/',
      tags: {
        english: 'some',
      },
    },
  ];
</script>

<section class="section">
  <div class="container is-fluid">
    <h1 class="title">Sites</h1>

    {#each sites as site}
      <article class="message">
        <div class="message-header">
          <p>{site.name}</p>
        </div>
        <div class="message-body">
          <TagList tags={site.tags}/>

          <div class="content">
            {@html site.description}

            <p><a href={site.href}>{site.href}</a></p>
          </div>
        </div>
      </article>
    {/each}
  </div>
</section>
