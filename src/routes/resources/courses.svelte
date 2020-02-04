<script>
  import Page from '../../components/ResourcePage.svelte';

  const courses = [
    {
      name: 'Duolingo',
      description: `<p>Probably the most popular language learning site.</p>`,
      href: 'https://www.duolingo.com/',
      tags: {
        apps: 'yes',
        audio: 'text-to-speech',
        bokmål: 'yes',
        free: 'yes',
        nynorsk: 'no',
        video: 'no',
      },
    },
    {
      name: 'Memrise',
      description: `<p>Somewhat of a very advanced flash-carding application.</p>`,
      href: 'https://www.memrise.com/',
      tags: {
        apps: 'paid',
        audio: 'yes',
        bokmål: 'yes',
        free: 'yes',
        nynorsk: 'no',
        video: 'paid',
      },
    },
    {
      name: 'Norwegian on the Web',
      description: `<p>NTNU's free introductory course to Norwegian.</p>`,
      href: 'https://www.ntnu.edu/now',
      tags: {
        apps: 'no',
        audio: 'yes',
        bokmål: 'yes',
        free: 'yes',
        nynorsk: 'no',
        video: 'no',
      },
    },
  ];
</script>

<Page items={courses} title="Courses"/>
