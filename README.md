# Kotatsu Club

This blog is a static content site built with [hugo](https://gohugo.io/). 

The theme is included as a submodule. Be sure to use the `--recursive` flag when cloning this repository.

Post content is written in [markdown](https://gohugo.io/content-management/formats/#learn-markdown).

### Create a post using the hugo cli
See [this](https://gohugo.io/getting-started/installing) page for hugo installation docs.

Run the `hugo new` command from the root directory of this repository.
```
hugo new --kind post-bundle post/your-nice-title
```
This will create a new directory `your-nice-title` and pre-populate the `index.md` file with the date and post title `Your Nice Title`. Populate the author key with the name you use for all your posts.

`--kind post-bundle` tells hugo which [archetype](https://github.com/kotatsuclub/hugo-theme-kotatsu/tree/master/archetypes) template to use when creating your index.md file.

### Create a post manually
If you do not wish to install the hugo cli you may create a post manually.
1. Create a new directory within [/content/post](/content/post). Give the directory a unique lowercase name and use dashes for spaces. 
2. Create an index.md file within your post directory and add the appropriate [front matter](https://gohugo.io/content-management/front-matter/):

```
+++
author = "bnVi"
date = 2020-01-11
title = "Example Post"
cover = "assets/hHovGdFGR.gif"
tags = ["example", "demo"]
+++
```
Supported front matter keys are:
* `author` - The name you want to publish as.
* `date` - The publish date for your post.
* `title` - Your post title.
* `cover` - A cover image for your post. Will only appear in home page summaries.
* `tags` - An array of tags you can use to categorize your posts.
* `draft` - When set to `true` your post will not be published.
* `disableDisqus` - When set to `true` disqus comments will be disabled for your post.

### Adding images, gifs, or other assets

When adding new images, gifs, or other assets it's best to download them and place them in an assets folder within your post directory rather than linking to an external site. This is to take advantage of better caching and ensure assets aren't lost when links disappear. 

### Shortcodes
Add [shortcodes](https://gohugo.io/content-management/shortcodes/) to your post content for figures with captions, embedded youtube videos, etc. 

```
{{< figure src="assets/N9D8i2F.png" caption="Is clockwise your left or my right?">}}

{{< youtube zAlJ9qhr2wA >}}
```

### Run the blog locally
Run `hugo serve` from the root directory of this repository. The first build will take some time to perform image resizing. Subsequent builds will utilize a resource cache. 

When the site finishes building it will be available at http://localhost:1313/. Hugo will automatically detect content changes and reload the site.