<template>
    <div>
        <header id="header">
            <nav id="main-menu">
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="about.html">About Me</a></li>
                    <li><a href="portfolio.html">Portfolio</a></li>
                    <li><a href="contact.html">Get in Touch</a></li>
                </ul>
            </nav>
            <img id="logo"
                src="img/me.png"
                alt="This is me.">
        </header>

        <nuxt />

        <footer id="footer" />
    </div>

</template>

<style lang="scss">
    @import '~assets/sass/main.scss';
    html {
        font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
            'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
        font-size: 16px;
        word-spacing: 1px;
        -ms-text-size-adjust: 100%;
        -webkit-text-size-adjust: 100%;
        -moz-osx-font-smoothing: grayscale;
        -webkit-font-smoothing: antialiased;
        box-sizing: border-box;
    }

    body {
        font-family: $text-font;
        color: $text-color;

        @include large-screens {
            font-size: 125%;
        }
    }

    h1,
    h2,
    h3,
    h4 {
        font-family: $headline-font;
    }

    p {
        font-family: $text-font;
    }

    a {
        color: $link-color;
    }

    @include fancy-links;

    #header {
        @include box(7px);
        @include box-shadow(2px 0px 4px#999, 1px 1px 6px $secondary-color);
        height: $header-height;
        background-color: $theme-color;

        #main-menu {
            li {
                display: inline;
            }
            a {
                color: $menu-item-color;
            }
        }
    }

    #footer {
        height: $footer-height;
        background-color: $ternary-color;
    }
    *,
    *:before,
    *:after {
        box-sizing: border-box;
        margin: 0;
    }

    .button--green {
        display: inline-block;
        border-radius: 4px;
        border: 1px solid #3b8070;
        color: #3b8070;
        text-decoration: none;
        padding: 10px 30px;
    }

    .button--green:hover {
        color: #fff;
        background-color: #3b8070;
    }

    .button--grey {
        display: inline-block;
        border-radius: 4px;
        border: 1px solid #35495e;
        color: #35495e;
        text-decoration: none;
        padding: 10px 30px;
        margin-left: 15px;
    }

    .button--grey:hover {
        color: #fff;
        background-color: #35495e;
    }
</style>
