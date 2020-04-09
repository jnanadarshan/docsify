# Doc helper

docsify extends Markdown syntax to make your documents more readable.

> Note: For the special code syntax cases, you'd better put them within a code backticks to avoid any conflicting from configurations or emojis.

## important content

Important content like:

```text
!> **Time** is money, my friend!
```

is rendered as:

!&gt; **Time** is money, my friend!

## General tips

General tips like:

```text
?> _TODO_ unit test
```

are rendered as:

?&gt; _TODO_ unit test

## Ignore to compile link

Some time we will put some other relative path to the link, you have to need to tell docsify you don't need to compile this link. For example

```text
[link](/demo/)
```

It will be compiled to `<a href="/#/demo/">link</a>` and will be loaded `/demo/README.md`. Maybe you want to jump to `/demo/index.html`.

Now you can do that

```text
[link](/demo/ ':ignore')
```

You will get `<a href="/demo/">link</a>`html. Do not worry, you can still set title for link.

```text
[link](/demo/ ':ignore title')

<a href="/demo/" title="title">link</a>
```

## Set target attribute for link

```text
[link](/demo ':target=_blank')
[link](/demo2 ':target=_self')
```

## Disable link

```text
[link](/demo ':disabled')
```

## Github Task Lists

```text
- [ ] foo
- bar
- [x] baz
- [] bam <~ not working
  - [ ] bim
  - [ ] lim
```

* [ ] foo
* bar
* [x] baz
* \[\] bam &lt;~ not working
  * [ ] bim
  * [ ] lim

## Image

### Resizing

```text
![logo](https://docsify.js.org/_media/icon.svg ':size=WIDTHxHEIGHT')
![logo](https://docsify.js.org/_media/icon.svg ':size=50x100')
![logo](https://docsify.js.org/_media/icon.svg ':size=100')

<!-- Support percentage -->

![logo](https://docsify.js.org/_media/icon.svg ':size=10%')
```

![:size=50x100](https://docsify.js.org/_media/icon.svg) ![:size=100](https://docsify.js.org/_media/icon.svg) ![:size=10%](https://docsify.js.org/_media/icon.svg)

### Customise class

```text
![logo](https://docsify.js.org/_media/icon.svg ':class=someCssClass')
```

### Customise ID

```text
![logo](https://docsify.js.org/_media/icon.svg ':id=someCssId')
```

## Customise ID for headings

```text
### 你好，世界！ :id=hello-world
```

## Markdown in html tag

You need to insert a space between the html and markdown content. This is useful for rendering markdown content in the details element.

```text
<details>
<summary>Self-assessment (Click to expand)</summary>

- Abc
- Abc

</details>
```

Self-assessment \(Click to expand\) - Abc - Abc

Or markdown content can be wrapped in html tag.

```text
<div style='color: red'>

- listitem
- listitem
- listitem

</div>
```

 - Abc - Abc

