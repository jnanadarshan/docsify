# Themes

There is a handful of themes available, both official and community-made. Copy [Vue](https://github.com/jnanadarshan/docsify/tree/e0e70dea214b0bf6b49a3dca8b0c394b18a3ca00/vuejs.org) and [buble](https://github.com/jnanadarshan/docsify/tree/e0e70dea214b0bf6b49a3dca8b0c394b18a3ca00/buble.surge.sh) website custom theme and [@liril-net](https://github.com/liril-net) contribution to the theme of the black style.

```markup
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/vue.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/buble.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/dark.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/pure.css">
```

!&gt; Compressed files are available in `/lib/themes/`.

```markup
<!-- compressed -->

<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/vue.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/buble.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/dark.css">
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/lib/themes/pure.css">
```

If you have any ideas or would like to develop a new theme, you are welcome to submit a [pull request](https://github.com/docsifyjs/docsify/pulls).

### Click to preview

 [vue.css](themes.md) [buble.css](themes.md) [dark.css](themes.md) [pure.css](themes.md)

  
  .demo-theme-preview a {  
    padding-right: 10px;  
  }  
  
  .demo-theme-preview a:hover {  
    cursor: pointer;  
    text-decoration: underline;  
  }  


  
  var preview = Docsify.dom.find\('.demo-theme-preview'\);  
  var themes = Docsify.dom.findAll\('\[rel="stylesheet"\]'\);  
  
  preview.onclick = function \(e\) {  
    var title = e.target.getAttribute\('data-theme'\)  
  
    themes.forEach\(function \(theme\) {  
      theme.disabled = theme.title !== title  
    }\);  
  };  


## Other themes

* [docsify-themeable](https://jhildenbiddle.github.io/docsify-themeable/#/) A delightfully simple theme system for docsify.

