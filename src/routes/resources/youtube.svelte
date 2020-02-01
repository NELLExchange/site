<script>
  import TagList from '../../components/TagList.svelte';

  const channels = [
    {
      name: 'Learn Norwegian Naturally',
      description: `<p>Topical videos mainly in Norwegian but with English subtitles.</p>`,
      href: 'https://www.youtube.com/user/NorwegianLearning',
      tags: {
        english: 'subtitles',
        learning: true,
      },
    },
    {
      name: 'Norsklærer Karense',
      description: `<p>Karense is a Norewgian teacher whose channel is aimed at teaching Norwegian.</p><p>While most of her videos are in Norwegian, she tends to use simple language.</p>`,
      href: 'https://www.youtube.com/channel/UCbrUYR892qBNQyY3DEqfTBg',
      tags: {
        english: 'some',
        learning: true,
      },
    },
    {
      name: 'Norwegian Teacher - Karin',
      description: `<p>Karin's channel is also aimed at teaching Norwegian with the majority of her content being explained in English.</p>`,
      href: 'https://www.youtube.com/user/Crienexzy',
      tags: {
        english: 'mostly',
        learning: true,
      },
    },
    {
      name: 'Peppa Gris - På Norsk',
      description: `<p>Official channel for Peppa Pig (children's television program) content in Norwegian.</p>`,
      href: 'https://www.youtube.com/channel/UC3oJMdoFT1NeygFutx4VhIg',
      tags: {
        english: false,
        learning: false,
      },
    },
  ];
</script>

<section class="section">
  <div class="container is-fluid">
    <h1 class="title">YouTube Channels</h1>

    {#each channels as channel}
      <article class="message">
        <div class="message-header">
          <p>{channel.name}</p>
        </div>
        <div class="message-body">
          <TagList tags={channel.tags}/>

          <div class="content">
            {@html channel.description}

            <p><a href={channel.href}>{channel.href}</a></p>
          </div>
        </div>
      </article>
    {/each}
  </div>
</section>
