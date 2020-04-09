# Embed files

With docsify 4.6 it is now possible to embed any type of file. You can embed these files as video, audio, iframes, or code blocks, and even Markdown files can even be embedded directly into the document.

For example, here embedded a Markdown file. You only need to do this:

```text
[filename](_media/example.md ':include')
```

Then the content of `example.md` will be displayed directly here

[filename](_media/example.md)

You can check the original content for [example.md](_media/example.md).

Normally, this will compiled into a link, but in docsify, if you add `:include` it will be embedded.

## Embedded file type

Currently, file extension are automatically recognized and embedded in different ways.

This is a supported embedding type:

* **iframe** `.html`, `.htm`
* **markdown** `.markdown`, `.md`
* **audio** `.mp3`
* **video** `.mp4`, `.ogg`
* **code** other file extension

Of course, you can force the specified. For example, you want to Markdown file as code block embedded.

```text
[filename](_media/example.md ':include :type=code')
```

You will get it

[filename](_media/example.md)

## Embedded code fragments

Sometimes you don't want to embed a whole file. Maybe because you need just a few lines but you want to compile and test the file in CI.

```text
[filename](_media/example.js ':include :type=code :fragment=demo')
```

In your code file you need to surround the fragment between `/// [demo]` lines \(before and after the fragment\).  
Alternatively you can use `### [demo]`.

Example:

[filename](https://github.com/jnanadarshan/docsify/tree/e0e70dea214b0bf6b49a3dca8b0c394b18a3ca00/docs/_media/example.js)

## Tag attribute

If you embed the file as `iframe`, `audio` and `video`, then you may need to set the attributes of these tags.

```text
[cinwell website](https://cinwell.com ':include :type=iframe width=100% height=400px')
```

[cinwell website](https://cinwell.com)

Did you see it? You only need to write directly. You can check [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe) for these attributes.

## The code block highlight

Embedding any type of source code file, you can specify the highlighted language or automatically identify.

```text
[](_media/example.html ':include :type=code text')
```

⬇️

?&gt; How to set highlight? You can see [here](language-highlight.md).

