<script>
  import TagList from './TagList.svelte';

  export let items;
  export let title;
</script>

<style>
  a {
    overflow-wrap: break-word;
    word-wrap: break-word;
  }

  @media screen and (max-width: 960px) {
    .container {
      padding-right: 0;
      padding-left: 0;
    }
  }
</style>

<section class="section">
  <div class="container is-fluid">
    <h1 class="title">{title}</h1>

    {#if items && items.length > 0}
    {#each items as item}
      <article class="message">
        <div class="message-header">
          <p>{item.name}</p>
        </div>
        <div class="message-body">
          <TagList tags={item.tags}/>

          <div class="content">
            {@html item.description}

            <p><a href={item.href}>{item.href}</a></p>
          </div>
        </div>
      </article>
    {/each}
    {/if}
  </div>
</section>
