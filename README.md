# bootstrap-chosen (less/sass)

![](https://github.com/alxlit/bootstrap-chosen/raw/master/example.png)

An alternate stylesheet for [Chosen 1.0](http://harvesthq.github.com/chosen/). This
one is supposed to integrate better with [Bootstrap 3.0](http://getbootstrap.com/).

[Here's the example page](http://alxlit.github.io/bootstrap-chosen/).

How you add `bootstrap-chosen.less` to your build process is up to you. Just keep
in mind that it needs access to `variables.less` and `mixins.less`.

You can tinker with the example page by:

```
$ git clone https://github.com/alxlit/bootstrap-chosen
$ cd bootstrap-chosen
bootstrap-chosen $ git clone --depth=1 https://github.com/twbs/bootstrap
bootstrap-chosen $ vi bootstrap/less/bootstrap.less

// Add this to the bottom
@import "../../bootstrap-chosen.less";

bootstrap-chosen $ lessc bootstrap/less/bootstrap.less > bootstrap.css
bootstrap-chosen $ firefox example.html
```

License: [MIT](https://en.wikipedia.org/wiki/MIT_License)

