+++
author = "bnVi"
date = 2020-01-11
title = "Example Post"
categories = ["bnVi", "example"]
+++

# Big fan

A post always begins with [front matter](ttps://gohugo.io/content-management/front-matter/).

```
+++
author = "bnVi"
date = 2020-01-11
title = "Example Post"
categories = ["example"]
+++
```

The post body is written in [markdown](https://gohugo.io/content-management/formats/#learn-markdown). Hugo [shortcodes](https://gohugo.io/content-management/shortcodes/) are available for things like figures with captions...

{{< figure src="https://i.imgur.com/N9D8i2F.png" caption="*Is clockwise your left or my right?*">}}

...and youtube videos
{{< youtube zAlJ9qhr2wA >}}


## How do I post?
Submit a pull request to the [content/post](https://github.com/kotatsuclub/blog/tree/master/content/post) directory in the [repo](https://github.com/kotatsuclub/blog). A preview link will be generated and attached to the pull request so you can see your post before it's live. If you have Hugo installed you can also clone/fork this repo and run `hugo server` to see your post as you write.
