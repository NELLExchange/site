<style global lang="scss">
  @charset 'utf-8';

  @import url('https://fonts.googleapis.com/css?family=Open+Sans&display=swap');

  $family-sans-serif: 'Open Sans', sans-serif;

  @import '../../node_modules/bulma/sass/utilities/_all.sass';
  @import '../../node_modules/bulma/sass/base/_all.sass';
  @import '../../node_modules/bulma/sass/components/_all.sass';
  @import '../../node_modules/bulma/sass/elements/_all.sass';
  @import '../../node_modules/bulma/sass/layout/_all.sass';
</style>

<script>
  import NavBar from '../components/NavBar.svelte'
</script>

<svelte:head>
  <title>Norwegian-English Language Learning Exchange</title>
</svelte:head>

<NavBar/>
<main>
  <slot></slot>
</main>
