# Hugo Reveal.js Generator

Simple presentation generator with [hugo](https://gohugo.io) and [reveal.js](http://lab.hakim.se/reveal-js/#/).

# How to use
1. [install hugo command](https://gohugo.io/overview/installing/)
2. create your workspace
  
  ```bash
  $ mkdir your-work-space && hugo new site your-work-space
  ```
3. install this theme

  ```bash
  $ cd your-work-space
  $ git clone https://github.com/minoritea/hugo-revealjs-generator themes/revealjs
  ```
  
4. add your first presentation

  ```bash
  $ hugo new your-presentation-name/slide1.md
  $ hugo new your-presentation-name/slide2.md
  $ hugo new your-presentation-name/slide3.md
  # ...
  ```

5. edit your slides
  - put your contents into slides in hugo's Markdown format.

  5.1. you can preview your slides on your computer
  
  ```bash
  $ hugo server -D -t revealjs # default URL is http://localhost:1313/
  ```

  
6. generate pages
  - don't forget to set `draft` as `false` in TOML headers in markdown files before publish them.
  
  ```bash
  $ hugo -t revealjs
  ```

7. put generated contents(in `public` directory) into your web site

# LISENCE
[MIT LISENCE](https://github.com/minoritea/hugo-revealjs-generator/blob/master/LICENSE.md)

Note: hugo and reveal.js have their own LISENCE.
