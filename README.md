# Simple 11ty example

This example is a minimal setup that lets you use JSON files (in `_data/`) as collections of data and [Nunjucks templating engine](https://mozilla.github.io/nunjucks/) to display that data on a website.

## Dev

Install with `npm install` and run with `npx @11ty/eleventy --serve` to start a dev server and `npx @11ty/eleventy` to build into `_site` that can be deployed to a server.

### CSS, Javascript and images

Anything stored in `assets/` folder will be copied as-is into `_site/assets` and not processed. To link to those in your templates or HTML, you can use `{{ '/assets/main.css' | url }}` that generates correct URLs (replace `main.css` with your filename).
