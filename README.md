# memoirs

Personal Web Blog

Defualt langauge on website is English.

Depolyed on ![github pages](https://github.com/py563/memoirs/actions/workflows/main.yml/badge.svg)

Current Theme [LoveIt](https://hugoloveit.com/)

## Creating New Posts

### Prefered

- Create a new folder in `posts` folder in `content` folder with same name as title of poems
- In name do not add space and replace it with hyphen `-` and try naming folder in english.
- create a file named `index.md` or `index.te.md` and write poem contents in it following below syntax.
- for english version create a file with name `index.en.md` in same folder.
- Add all related images about poem in the new folder, main image to be added in `featured-image`.

### Second way

- Create a new markdown file in `content` folder with same name as title of poem `poem-name.md`
- In name do not add space and replace it with hyphen `-`
- write poem or song or commentary by following below structure.
- For English version copy the file contents into new file named `poem-name.en.md`

## New Post Structure and Metadata

Always start new post with following lines then write actual content

```yml
---
weight: 1
title: "Post Name కవిత పేరు" # telugu name good
date: 2019-03-09 # replace with current date
draft: false # if poem is still a draft then change to true
tags: ["test"] # include related tags
categories: ["పాటలు"] # ఏ విభాగం కి
author: "author" # Telugu script good
authorLink: "something if available"
description: "Lorem Ipsum Dolor Si Amet." # post గురించి ఒక్క line లో
timeToRead: "10" # చదవడానికి అయే time estimate

resources:
  - name: "featured-image" # main image home పేజీ లో వస్తుంది
    src: "hero-4.jpg" # file పేరు & ఆ folder లో నే ఉండాలి

lightgallery: true
hiddenFromHomePage: false # books కి true -- home పేజీ లో కనపడకుండా చేస్తూంది

toc:
  auto: false # విషయ సూచిక కొరకు
---
హోం పేజీ లో టైటిల్ కింద చూపించే ఒక్క లైన్ <!--more-->

ఇక్కడ ఉంది రాయడం మొదలుపెట్టండి
```

When you want to hide it from home page like below

```yml
categories: ["Books"]
hiddenFromHomePage: true
```

## Creating new pages

- Create a new file with like `pagename.md` or `pagename.en.md` in `page` folder under `content`

- follow this structure

```yml
---
weight: 1
title: "పేజీ టైటిల్"
subtitle: "సబ్ టైటిల్ ఉంటే ఇక్కడ రాయండి"
date: 2019-03-06
draft: false
lightgallery: true
---
పేజీ కంటెంట్
```

## Helpful tips for writing in Hugo

- use `##` big heading like above section name or `###` or `####` for headings.

- to add new hyperlink like [google.com](https://www.google.com/) use:

```md
[google.com](https://www.google.com/)
```

- to add image use both local and from internet

```md
![Tux, the Linux mascot](/assets/images/tux.png)
![nidhi-logo](https://images.pexels.com/photos/207691/pexels-photo-207691.jpeg)
```

![nidhi-logo](https://images.pexels.com/photos/207691/pexels-photo-207691.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=457&w=640)

- to make text bold use `**bold text**` **bold text**.

- to make italic use `*cat's meow*` _cat's meow_.

- to make text bold and italic use `***cat's meow***` **_cat's meow_**.

- To create a blockquote, add a > in front of a paragraph.

`md > Dorothy followed her through many of the beautiful rooms in her castle.`

- to make list use `-` or number them

```md
- test 1
- test 2
  - test 2.1

1.  test 1
2.  test 2
3.  test 2.1
```

1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item

- To create a horizontal rule, use three or more dashes `---` on a line by themselves and put blank lines before and after horizontal rules.

  ***

- to add figure like charts or more than images use

```go
{{< figure src="/media/spf13.jpg" title="Steve Francia" >}}
```

- to include a single tweet into your blog post, we will need is the URL of the tweet: like this tweet id

<https://twitter.com/spf13/status/877500564405444608>

```go
{{< tweet 877500564405444608 >}}
```

- to include youtube video like this song use id of the video i.e text after ?v=

<https://www.youtube.com/watch?v=8PiwQJHtN8s>

```go
{{< youtube 8PiwQJHtN8s >}}
```

## LICENSE

MIT
