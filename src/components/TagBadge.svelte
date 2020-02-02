<script>
  export let name;
  export let value;

  const successValues = [true, 'mostly'];
  const warningValues = ['paid', 'some', 'subtitles', 'text-to-speech'];

  function getClass(value) {
    if (successValues.includes(value)) {
      return 'is-success';
    }

    if (warningValues.includes(value)) {
      return 'is-warning';
    }

    return 'is-danger';
  }

  function getValue(value) {
    if (value === true) {
      return 'yes';
    }

    if (value === false) {
      return 'no';
    }

    return value;
  }
</script>

<span class="tag is-dark">{name}</span>
<span class="tag {getClass(value)}">{getValue(value)}</span>
