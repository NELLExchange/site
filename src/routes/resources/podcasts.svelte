<script>
  import Page from '../../components/ResourcePage.svelte';

  const sites = [
    {
      name: 'Abels Tårn',
      description: `<p>Weekly NRK podcast. Three researchers navigate through the jungle of alternative facts in search of the truth about how the world works, debating and answering questions from the audience.</p>`,
      href: 'https://radio.nrk.no/podkast/abels_taarn',
      tags: {
        level: 'intermediate',
        transcriptions: 'no'
      }
    },
    {
      name: 'Ekko',
      description: `<p>A daily (Monday to Saturday) NRK programme about society, with interviews, reports and more.</p>`,
      href: 'https://radio.nrk.no/serie/ekko',
      tags: {
        level: 'intermediate/advanced',
        transcriptions: 'no'
      }
    },
    {
      name: 'Lær Norsk Nå!',
      description: `<p>A podcast targeted at intermediate (B1-B2) learners, with transcriptions available. By Marius Stangeland.</p>`,
      href: 'https://laernorsknaa.wixsite.com/laernorsknaa',
      tags: {
        level: 'intermediate',
        transcriptions: 'yes',
      },
    },
    {
      name: 'Språkteigen',
      description: `<p>A weekly NRK podcast about new words and old words, new research and strange language phenomena. Recommended for advanced learners.</p>`,
      href: 'https://radio.nrk.no/podkast/spraakteigen',
      tags: {
        level: 'advanced',
        transcriptions: 'no'
      }
    },
    {
      name: 'Verdibørsen',
      description: `<p>Weekly NRK podcast. Ethical, moral, political and philosophical discussions over topics of worldview and life in a society.</p>`,
      href: 'https://radio.nrk.no/podkast/verdiboersen',
      tags: {
        level: 'advanced',
        transcriptions: 'no'
      }
    }
  ];
</script>

<Page items={sites} title="Podcasts"/>
