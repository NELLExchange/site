<script>
  import Page from './_page.svelte';

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

<Page items={sites} title="Sites"/>
