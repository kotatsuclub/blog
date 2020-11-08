# Kotatsu Club

To submit a post, add a `.md` file to the [/content/post](/content/post) directory. Give the file a unique lowercase name and use dashes for spaces. 

A post always begins with [front matter](https://gohugo.io/content-management/front-matter/).

```
+++
author = "bnVi"
date = 2020-01-11
title = "Example Post"
cover = "https://cdn.kotatsu.club/hHovGdFGR.gif"
categories = ["example", "demo"]
+++
```

The post body written in [markdown](https://gohugo.io/content-management/formats/#learn-markdown). Hugo [shortcodes](https://gohugo.io/content-management/shortcodes/) are available for figures with captions, youtube videos, etc. 

```
{{< figure src="https://i.imgur.com/N9D8i2F.png" caption="*Is clockwise your left or my right?*">}}

{{< youtube zAlJ9qhr2wA >}}
```

When adding new images or gifs it's best to link to an external site such as imgur rather than uploading them to this repo. After your post has been merged any external links will be copied to the Kotatsu Club CDN and replaced inline. 
