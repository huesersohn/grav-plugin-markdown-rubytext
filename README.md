# Grav Markdown RubyText Plugin

The **markdown-rubytext plugin** for [Grav](http://github.com/getgrav/grav) allows you to add output <ruby> tagged text in Markdown:

# Installation

This plugin is easy to install with GPM.

```
$ bin/gpm install markdown-rubytext
```

# Configuration

Simply copy the `user/plugins/markdown-color/markdown-rubytext.yaml` into `user/config/plugins/markdown-rubytext.yaml` and make your modifications.

```
enabled: true
```

#Usage

In your markdown file:

```
This is {r}日本語{/r:にほんご} and this is {r}漢{/r:ㄏㄢˋ}.
```

Will produce the following HTML:

```
This is <ruby><rb>日本語</rb><rt>にほんご</rt></ruby> and this is <ruby><rb>漢</rb><rt>ㄏㄢˋ</rt></ruby>.
```

Standart display:

![this-is-nihongo-and-this-is-kan](this-is-nihongo-and-this-is-kan.PNG)

## important note:
This plugin will not work without at least one space before: `space` + `{r}日本語{/r:にほんご}` in the markdown file.

## future development:
to make possible the same output without any `space` before the regular expression.
