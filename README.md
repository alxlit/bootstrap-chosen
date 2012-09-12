
# bootstrap-chosen.less

![](https://github.com/alxlit/bootstrap-chosen/raw/master/example.png)

An alternate stylesheet for [Chosen](http://harvesthq.github.com/chosen/). This
one is supposed to integrate better with Bootstrap.

Chosen widgets are given the `outerWidth` of the form element that they are
replacing. This can be ambiguous; to fix this, wrap them with
`<div class="chosen">...</div>`, or `chosen-mini`, `chosen-small`, etc.

If you want to compile it as a standalone, you'll need to add
`@import "variables.less";` and `@import "mixins.less";`.

If you want to mess around with the example page:

```
$ git clone git@github.com:twitter/bootstrap
```

Edit bootstrap.less to `@import "../../bootstrap-chosen.less";`. Then,

```
$ wget https://raw.github.com/harvesthq/chosen/master/chosen/chosen-sprite.png
$ lessc bootstrap/less/bootstrap.less > bootstrap.css
```

License: WTFPL

