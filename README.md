# Technical info

This site is built using [jekyllrb.com](https://jekyllrb.com/)

Any commits pushed to github or made directly on the site will be automatically
published on github pages after a short delay.

## Access

Any member of the OCCC is welcome to contribute to the site. Email the current
chair (see [the index](/index.html) for contact info) or anyone listed on the
[contributors](https://github.com/Oregon-Council-of-Computer-Chairs/Oregon-Council-of-Computer-Chairs.github.io/graphs/contributors) list of the repo for access.

## Adding pages

Any markdown file that does not begin with an underscore, and is not in a folder that begins with
an underscore, will be turned into an html page. Here is a [guide to GitHub's markdown
syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

If markdown is not sufficiently expressive, you can also embed html directly into a
markdown page. However, for ease of maintenance, avoid using html if markdown will
suffice for a purpose. To embed markdown inside of html, make sure to specify the attribute
`markdown="1"` in the enclosing html element. ([See docs](https://kramdown.gettalong.org/syntax.html#html-blocks))

Markdown files may have YAML formatted "front matter". In particular a **title** is
encouraged for all pages - it will automatically be rendered at the top of the page
as an &lt;h1&gt; tag.

    ---
    title: Sample page
    ---

## Previewing changes

Many editors offer markdown preview if you want to examine what you are producing.
You can also use the GitHub web interface to edit individual pages and preview the
markdown before committing. However, Jekyll supports advanced features that the
GitHub website does not. Fancier pages that render correctly on github pages
may not render correctly if previewed on GitHub.

If you want do more extensive editing and preview your changes, you may wish to install Jekyll to
build pages in the exact same way that the GitHub pages system will. You can find instructions for
doing so on the
[GitHub Test site locally with Jekyll docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

## Configuration and Site Navigation

The file [_config.yml](config.yml) contains high level options for the site. 
In particular, this is where the top navigation links are set from.

## Theme

Documentation for customizing the theme (mimia) can be found here:
https://www.rubydoc.info/gems/minima/2.5.1#Customization

The source code for Minima at GitHub:
[jekyll][jekyll-organization] /
[minima](https://github.com/jekyll/minima)

> **Note:**  The master branch of this project is often ahead of the version of minima
> currently available via ruby gems and in use on this site.