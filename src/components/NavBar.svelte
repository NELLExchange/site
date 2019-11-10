<script>
  function toggleNav() {
    document.getElementById('navMenu').classList.toggle('is-active');
  }
</script>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href=".">
      NELLE
    </a>

    <span role="button" class="navbar-burger burger" on:click={toggleNav} aria-label="menu" aria-expanded="false" data-target="navMenu">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </span>
  </div>

  <div id="navMenu" class="navbar-menu">
    <div class="navbar-start">
      <div class="navbar-item has-dropdown is-hoverable">
        <span class="navbar-link">
          Resources
        </span>

        <div class="navbar-dropdown">
          <a class="navbar-item" href="resources/dictionaries">
            Dictionaries
          </a>
        </div>
      </div>
    </div>
  </div>
</nav>
