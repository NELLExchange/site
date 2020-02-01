<script>
  export let name;
  export let value;

  const successValues = [true, 'mostly'];
  const warningValues = ['some', 'subtitles'];

  function getClass(value) {
    if (successValues.includes(value)) {
      return 'is-success';
    }

    if (warningValues.includes(value)) {
      return 'is-warning';
    }

    return 'is-danger';
  }
</script>

<span class="tag is-dark">{name}</span>
<span class="tag {getClass(value)}">{value}</span>
