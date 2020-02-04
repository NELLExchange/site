<script>
  import Page from '../../components/ResourcePage.svelte';

  const dictionaries = [
    {
      name: 'Universitet i Bergens Ordbok',
      description: `<p>The University of Bergen's dictionary.</p><p>Contains the official writing standard and all allowed variants of Norwegian.</p>`,
      href: 'https://ordbok.uib.no/',
      tags: {
        bokmål: 'yes',
        nynorsk: 'yes',
        english: 'no',
        examples: 'yes',
        inflections: 'yes',
      },
    },
    {
      name: 'LEXIN',
      description: `<p>A set of dictionaries designed for minority language speakers in Norway to help with learning everyday Norwegian.</p><p>The Nynorsk-Bokmål and English-Nynorsk dictionaries can be used together to get English-Bokmål translations.</p>`,
      href: 'https://lexin.oslomet.no/',
      tags: {
        bokmål: 'yes',
        nynorsk: 'yes',
        english: 'yes',
        examples: 'yes',
        inflections: 'yes',
      },
    },
    {
      name: 'Norske Akademis Ordbok',
      description: `<p>The Norwegian Academy's dictionary.</p><p>Contains a small sub-set of 'moderat' bokmål and riksmål (not official).</p><p>This makes this dictionary better at handling slang.</p>`,
      href: 'https://www.naob.no/ordbok/',
      tags: {
        bokmål: 'yes',
        nynorsk: 'no',
        english: 'no',
        examples: 'yes',
        inflections: 'yes',
      },
    },
    {
      name: 'bab.la',
      description: `<p>bab.la's Norwegian-English dictionary.</p><p>If you need English translations of words, this site often does a better job than Google Translate.</p>`,
      href: 'https://en.bab.la/dictionary/norwegian-english/',
      tags: {
        bokmål: 'yes',
        nynorsk: 'no',
        english: 'yes',
        examples: 'yes',
        inflections: 'no',
      },
    },
  ];
</script>

<Page items={dictionaries} title="Dictionaries"/>
