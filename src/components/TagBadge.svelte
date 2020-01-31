<script>
  export let name;
  export let value;

  const successValues = [true];
</script>

<span class="tag is-dark">{name}</span>
<span class="tag {successValues.includes(value) ? 'is-success' : 'is-danger'}">{value}</span>
