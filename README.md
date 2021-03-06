# [jQuery](http://jquery.com) Snippets for [Atom](http://atom.io)

<!---
## Install

Go to `Atom > Preferences...` then search for **JavaScript Snippets** in Packages tab.
Restart atom.
--->
## Install

```sh
$ cd ~/.atom/packages
$ git clone https://github.com/brandontrowe/atom-jquery-snippets.git
$ cd atom-jquery-snippets
$ apm install
$ apm link
```
## Snippets

### [jquery] $(function(){})

```javascript
$(function() {
    ${1:// body...}
});
```

### [ajax] jQuery.ajax()

```javascript
$.ajax({
    method: '${1:GET}',
    url: ${2:/},
    dataType: '${3:json}',
    data: '${4:data}',
})
.done(function( data ) {
    ${5://data...}
})
.fail(function( jqXHR, textStatus ) {
    console.error( "Request failed: " + textStatus );
});
```

### [extend] jQuery.fn.extend()

```javascript
$.fn.extend({
    ${1:methodName}: function (${2:options}) {
        ${3://body...}
    }
});
```

## Develop and Contribute

1. Fork it
2. Clone your repo fork
3. Create your feature branch: `git checkout -b my-new-feature`
4. Commit your changes: `git commit -m 'Add some feature'`
5. Push to the branch: `git push origin my-new-feature`
6. Submit a pull request

## Based on [Javascript Snippets for Atom](https://github.com/zenorocha/atom-javascript-snippets) by Zeno Rocha
