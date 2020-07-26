<script>
  import Page from '../../components/ResourcePage.svelte';

  const sites = [
    {
      name: 'Lær Norsk Nå!',
      description: `<p>A podcast targeted at intermediate (B1-B2) learners, with transcriptions available. By Marius Stangeland.</p>`,
      href: 'https://laernorsknaa.wixsite.com/laernorsknaa',
      tags: {
        transcriptions: 'yes',
      },
    },
  ];
</script>

<Page items={sites} title="Podcasts"/>
