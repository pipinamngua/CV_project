<template>
  <div id="main"
    role="main">

    <article id="content">
      <h1>Welcome to My Site!</h1>
      <section id="introduction">
        <h2>Hi, I am Mr. Website!</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Qui pariatur in iure. Rem, aliquid, cumque. Id tenetur, facere aut odio dolores qui, iste sit voluptates ullam doloribus suscipit quasi obcaecati alias voluptatum error ab <a href="#">repellendus</a> deleniti ipsa quae sint! Nobis tempora cupiditate voluptate earum fuga laudantium vitae deleniti consectetur sapiente.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptas possimus, et deleniti commodi sit, excepturi! Perspiciatis omnis aut impedit saepe consequatur quis dolores distinctio cumque aperiam velit repellendus dicta temporibus, a ducimus exercitationem, ratione harum quos voluptatem totam possimus eaque, porro quo voluptatum voluptates. Ducimus facere quod laborum, odit numquam amet. Ea sequi, harum neque, alias ratione iure blanditiis, accusamus reprehenderit impedit numquam libero suscipit voluptatibus enim. Exercitationem placeat, repellat.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Suscipit, eius sapiente excepturi saepe vero maxime! Laborum quidem debitis labore quia magni tempore <a href="#">voluptatibus</a> omnis pariatur consectetur, molestiae nisi et ratione?</p>
      </section>
      <section id="promo">
        <h2>Check Out My Work</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex omnis atque illo odio labore, debitis, qui quo? Odio similique illum eligendi distinctio repellendus quod inventore, aliquam modi, recusandae labore dignissimos aperiam expedita unde ea rem iusto magni ipsum nisi neque!</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsam eum quod et provident consectetur dolores, itaque quae <a href="#">dignissimos voluptatem</a>, accusamus, aut omnis ipsa quidem error magni facilis excepturi explicabo repudiandae. Velit beatae, facere magni. Odio obcaecati possimus reiciendis incidunt quo expedita quis ipsum quibusdam omnis, numquam beatae minima iure tenetur impedit totam ea esse deleniti eum? Minima maiores expedita, accusamus.</p>
      </section>
    </article>

    <aside id="sidebar">
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
      </ul>
    </aside>

  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="scss">
  @import '~assets/sass/main.scss';
  #main {
      width: $content-width;
      height: auto;
      @include large-screens {
          width: auto;
          max-width: $content-width;
      }
      margin-left: auto;
      margin-right: auto;

      #content {
      }

      #sidebar {
      }
  }
  .container {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
  }

  .title {
      font-family: 'Quicksand', 'Source Sans Pro', -apple-system,
          BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial,
          sans-serif;
      display: block;
      font-weight: 300;
      font-size: 100px;
      color: #35495e;
      letter-spacing: 1px;
  }

  .subtitle {
      font-weight: 300;
      font-size: 42px;
      color: #526488;
      word-spacing: 5px;
      padding-bottom: 15px;
  }

  .links {
      padding-top: 15px;
  }
</style>
