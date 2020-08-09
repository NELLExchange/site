<script>
  import TagBadge from './TagBadge.svelte';

  export let tags;
</script>

<div class="field is-grouped is-grouped-multiline">
  {#each Object.keys(tags || {}) as tag}
    <div class="control">
      <div class="tags has-addons">
        <TagBadge name={tag} value={tags[tag]}/>
      </div>
    </div>
  {/each}
</div>
