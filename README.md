# bootstrap-chosen.less

![](https://github.com/alxlit/bootstrap-chosen/raw/master/example.png)

An alternate stylesheet for [Chosen](http://harvesthq.github.com/chosen/). This
one is supposed to integrate better with Bootstrap.

## Usage

Chosen widgets are given the `outerWidth` of the form element that they are
replacing, which is ambiguous and often not what you'd expect. Wrap them with
the "chosen" class (or chosen-mini, chosen-small, etc) to fix this.

```html
<div class="chosen">
  <select class="chzn-select">
    <option>...</option>
  </select>
</div>
```

How you add `bootstrap-chosen.less` to you build process is up to you. Just keep in mind
that it needs access to `variables.less` and `mixins.less`.

## Development

Set up the example page by:

```
$ git clone https://github.com/alxlit/bootstrap-chosen
$ cd bootstrap-chosen
bootstrap-chosen $ git clone https://github.com/twitter/bootstrap
bootstrap-chosen $ vi bootstrap/less/bootstrap.less

// Add this to the bottom
@import "../../bootstrap-chosen.less";

bootstrap-chosen $ lessc bootstrap/less/bootstrap.less > bootstrap.css
bootstrap-chosen $ firefox example.html
```

License: [MIT](https://en.wikipedia.org/wiki/MIT_License)

