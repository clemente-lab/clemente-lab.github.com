# Clemente Lab Website

## Instructions

To build and view locally, comment-out the ```url:``` line in ```_config.yml```
and run:

```jekyll serve -w```

Then browse to ```localhost:4000``` to view the website.

To make changes to the CSS, you'll need to install ```lessc``` in order to
compile the LESS code into CSS. Once you're done making changes to the
```LESS``` files, run the following command (assuming you are at the root of
the repository):

```lessc assets/less/main.less assets/css/main.css```

## Acknowledgements

This website makes use of the following tools/resources:

* [Jekyll](http://jekyllrb.com/)
* [So Simple Theme](http://mademistakes.com/articles/so-simple-jekyll-theme.html)
* [pubmed-js](https://github.com/ebolyen/pubmed-js)
* Loading icons provided by [mentalized.net](http://mentalized.net/activity-indicators/)

## License

This website is free and open source, made available via the
[GNU General Public License](LICENSE) version 2 or later.
