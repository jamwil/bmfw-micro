# Better Motherfucking Website — a Micro.blog theme

A [Micro.blog](https://micro.blog) compatible [Hugo](https://gohugo.io) theme based on
[bettermotherfuckingwebsite.com](http://bettermotherfuckingwebsite.com/).

It starts with the original **7 declarations**:

```css
body {
	margin: 40px auto;
	max-width: 650px;
	line-height: 1.6;
	font-size: 18px;
	color: #444;
	padding: 0 10px;
}

h1, h2, h3 {
	line-height: 1.2;
}
```

…then adds only the minimal extras a blog actually needs: images that don't
overflow the layout, readable quotes and code, a photos grid, and pagination.
No webfonts. No JavaScript. No frameworks. Still loads instantly.

## Features

* Micro posts (titleless posts) and full posts, rendered with [microformats2](http://microformats.org/wiki/microformats2) (`h-feed`, `h-entry`)
* Replies section with `u-in-reply-to` context
* Photos page (`/photos`) and archive page (`/archive`)
* Categories
* RSS feed, [JSON Feed](https://jsonfeed.org), podcast feeds (XML + JSON)
* IndieWeb endpoints in `<head>`: Micropub, IndieAuth, Webmention, Microsub, `rel=me`
* Pagination (enable with Micro.blog's `paginate_home`, `paginate_categories`, `paginate_replies` settings)
* Micro.blog plug-in hooks (`plugins_css`, `plugins_js`, `plugins_html`, custom footer)

## Installation on Micro.blog

1. Sign in to Micro.blog and go to **Plug-ins**.
2. Click **Find Plug-ins**, scroll to the bottom, and paste this repository's URL
   into **Install from a GitHub URL**.
3. Go to **Design** and select **Better Motherfucking Website** as your blog's theme.

## Using it as a plain Hugo theme

Clone it into your site's `themes` directory and set `theme = "bmfw-micro"` in
your config. Micro.blog-specific params (`author`, `theme_seconds`, `site_id`,
`itunes_*`, …) are injected by Micro.blog at build time; locally you can define
them yourself or ignore them.

## Inspiration

* [motherfuckingwebsite.com](http://motherfuckingwebsite.com/)
* [bettermotherfuckingwebsite.com](http://bettermotherfuckingwebsite.com/)

## License

MIT
