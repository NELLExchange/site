<style lang="scss">
  .has-background {
    background: url('../splash.jpg') center center/cover no-repeat;
  }

  .hero-body > .container {
    background: rgba(#000000, 0.5);
    border-radius: 1em;
    padding: 1em;
  }

  .subtitle, .title {
    text-shadow: 2px 2px #000000;
  }

  #appropriation {
    color: white;
    display: inline-block;
    font-size: 12px;
    font-weight: bold;
    line-height: 1.2;
    padding: 4px 6px;
    text-decoration:none;

    #appropriation-logo {
      display: inline-block;
      padding: 2px 3px;

      > svg {
        fill: white;
        height: 12px;
        position: relative;
        top: -2px;
        vertical-align: middle;
        width: auto;
      }
    }

    #appropriation-author {
      display: inline-block;
      padding: 2px 3px;
    }
  }
</style>

<section class="hero is-dark is-fullheight-with-navbar has-background">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        Norwegian-English Language Learning Exchange
      </h1>
      <h2 class="subtitle">
        Welcome to NELLE!
      </h2>
    </div>
  </div>
  <div class="hero-foot">
    <a id="appropriation"
       class="is-pulled-right"
       href="https://unsplash.com/@ygar?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge"
       rel="noopener noreferrer"
       target="_blank"
       title="Download free do whatever you want high-resolution photos from Yuriy Garnaev">
      <span id="appropriation-logo">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
          <title>unsplash-logo</title>
          <path d="M10 9V0h12v9H10zm12 5h10v18H0V14h10v9h12v-9z"></path>
        </svg>
      </span>
      <span id="appropriation-author">Yuriy Garnaev</span>
    </a>
  </div>
</section>
