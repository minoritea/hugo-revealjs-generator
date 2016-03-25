# Hugo Reveal.js Generator

Simple presentation generator with [hugo](https://gohugo.io) and [reveal.js](http://lab.hakim.se/reveal-js/#/).

An example is here. [https://tanstaafl.0pt.jp/slides/](https://tanstaafl.0pt.jp/slides/)

# How to use
1. [Install hugo command](https://gohugo.io/overview/installing/).
2. Create your workspace.
  
  ```bash
  $ mkdir your-work-space && hugo new site your-work-space
  ```
3. Install this theme.

  ```bash
  $ cd your-work-space
  $ git clone https://github.com/minoritea/hugo-revealjs-generator themes/revealjs
  ```
  
4. Add your first presentation.

  ```bash
  $ hugo new your-presentation-name/slide1.md
  $ hugo new your-presentation-name/slide2.md
  $ hugo new your-presentation-name/slide3.md
  # ...
  ```
  Note that your slides are sorted by title(e.g. slide1 > slide2 > slide3 ...).

5. edit your slides.
  - put your contents into slides in hugo's Markdown format.

  5.1. You can preview your slides on your computer.
  
  ```bash
  $ hugo server -D -t revealjs # default URL is http://localhost:1313/
  ```

  
6. Generate pages.
  - don't forget to set `draft` as `false` in TOML headers in markdown files before publish them.
  
  ```bash
  $ hugo -t revealjs
  ```

7. Put generated contents(in `public` directory) into your web site.

# LISENCE
[MIT LISENCE](https://github.com/minoritea/hugo-revealjs-generator/blob/master/LICENSE.md)

Note: hugo and reveal.js have their own LISENCE.
