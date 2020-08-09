<script>
  import Page from '../../components/ResourcePage.svelte';

  const sites = [
    {
      name: 'grammatikk.com',
      description: `<p>Short Norwegian grammar cheat-sheets.</p>`,
      href: 'http://grammatikk.com/',
      tags: {
        english: 'some',
        bokmål: 'yes',
        nynorsk: 'no'
      },
    },
    {
      name: 'Nynorskartiklar hos NRK',
      description: `<p>A searchable feed of Nynorsk articles in NRK, updated daily. By user Henbruas.</p>`,
      href: 'https://nrknynorsk.duckdns.org/',
      tags: {
        english: 'no',
        bokmål: 'no',
        nynorsk: 'yes'
      }
    }
  ];
</script>

<Page items={sites} title="Sites"/>
