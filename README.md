# grunt-assemble-navigation [![NPM version](https://badge.fury.io/js/grunt-assemble-navigation.svg)](http://badge.fury.io/js/grunt-assemble-navigation)

> Assemble navigation plugin. Automatically generate Bootstrap-style, multi-level side nav. See the sidenav on assemble.io for a demonstration.

**Here's a preview**

![image](https://f.cloud.github.com/assets/383994/2523672/94f62414-b4d4-11e3-98c6-fc3c07bef4b4.png)

***

## Quickstart

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i grunt-assemble-navigation --save
```

## Usage

Register the middleware with Assemble:

```js
options: {
  plugins: ['grunt-assemble-navigation', 'foo/*.js']
}
```

Visit the [plugins docs](http://assemble.io/plugins/) for more info or for help getting started.

Add this markup where you want the navigation:

```html
<div id="navigation">
  <!-- navigation -->
</div>
```

The plugin uses page headings to construct the nav items, results in something like:

```html
<div id="navigation">
  <!-- navigation -->
  <ul class="nav sidenav">
    <li><a href="#collections">Collections</a>
      <ul class="nav">
        <li> <a href="#collections-after">{{after}}</a> </li>
        <li> <a href="#collections-any">{{any}}</a> </li>
        <li> <a href="#collections-before">{{before}}</a> </li>
      </ul>
    </li>
  </ul>
</div>
```

***

## Other grunt-assemble middleware

* [grunt-assemble](https://www.npmjs.com/package/grunt-assemble): Static site generator for Grunt.js, Yeoman and Node.js. Used by Zurb Foundation, Zurb Ink, H5BP/Effeckt,… [more](https://www.npmjs.com/package/grunt-assemble) | [homepage](http://assemble.io)
* [grunt-assemble-anchors](https://www.npmjs.com/package/grunt-assemble-anchors): Assemble plugin for creating anchor tags from headings in generated html using Cheerio.js. | [homepage](https://github.com/assemble/grunt-assemble-anchors)
* [grunt-assemble-contextual](https://www.npmjs.com/package/grunt-assemble-contextual): Generates a JSON file with the context of each page. Basic plugin to help see… [more](https://www.npmjs.com/package/grunt-assemble-contextual) | [homepage](https://github.com/assemble/grunt-assemble-contextual)
* [grunt-assemble-decompress](https://www.npmjs.com/package/grunt-assemble-decompress): Assemble plugin for extracting zip, tar and tar.gz archives. | [homepage](https://github.com/assemble/grunt-assemble-decompress)
* [grunt-assemble-download](https://www.npmjs.com/package/grunt-assemble-download): Assemble plugin for downloading files from GitHub. | [homepage](https://github.com/assemble/grunt-assemble-download)
* [grunt-assemble-i18n](https://www.npmjs.com/package/grunt-assemble-i18n): Plugin for adding i18n support to Assemble projects. | [homepage](https://github.com/assemble/grunt-assemble-i18n)
* [grunt-assemble-lunr](https://www.npmjs.com/package/grunt-assemble-lunr): Assemble plugin for adding search capabilities to your static site, with lunr.js. | [homepage](http://assemble.io)
* [grunt-assemble-permalinks](https://www.npmjs.com/package/grunt-assemble-permalinks): Permalinks plugin for Assemble, the static site generator for Grunt.js, Yeoman and Node.js. This plugin… [more](https://www.npmjs.com/package/grunt-assemble-permalinks) | [homepage](https://github.com/assemble/grunt-assemble-permalinks)
* [grunt-assemble-sitemap](https://www.npmjs.com/package/grunt-assemble-sitemap): Sitemap plugin for Assemble | [homepage](http://assemble.io/plugins)
* [grunt-assemble-toc](https://www.npmjs.com/package/grunt-assemble-toc): Assemble middleware for adding a Table of Contents (TOC) to any HTML page. | [homepage](http://assemble.io)
* [grunt-assemble-wordcount](https://www.npmjs.com/package/grunt-assemble-wordcount): Assemble plugin for displaying wordcount and average reading time to blog posts or pages. | [homepage](https://github.com/assemble/grunt-assemble-wordcount)

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/assemble/grunt-assemble-navigation/issues/new).

## Authors

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on September 25, 2015._