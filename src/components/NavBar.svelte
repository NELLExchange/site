<script>
  function toggleNav() {
    const { target } = this.dataset;
    const $target = document.getElementById(target);
    
    this.classList.toggle('is-active');
    $target.classList.toggle('is-active');
  }
</script>

<nav class="navbar is-dark is-fixed-top" role="navigation" aria-label="main navigation">
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
          Discord
        </span>

        <div class="navbar-dropdown">
          <a class="navbar-item" href="https://discord.gg/2d37xPa">
            Join the Server
          </a>
        </div>
      </div>

      <div class="navbar-item has-dropdown is-hoverable">
        <span class="navbar-link">
          Resources
        </span>

        <div class="navbar-dropdown">
          <a class="navbar-item" href="resources/courses">
            Courses
          </a>

          <a class="navbar-item" href="resources/dictionaries">
            Dictionaries
          </a>
          
          <a class="navbar-item" href="resources/podcasts">
            Podcasts
          </a>

          <a class="navbar-item" href="resources/sites">
            Sites
          </a>

          <a class="navbar-item" href="resources/youtube">
            YouTube
          </a>
        </div>
      </div>
    </div>
  </div>
</nav>
