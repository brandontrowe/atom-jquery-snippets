# [jQuery](http://jquery.com) Snippets for [Atom](http://atom.io)

<!---
## Install

Go to `Atom > Preferences...` then search for **JavaScript Snippets** in Packages tab.
Restart atom.
--->

## Development

```sh
$ cd ~/.atom/packages
$ git clone https://github.com/brandontrowe/atom-jquery-snippets.git
$ cd atom-jquery-snippets
$ apm install
$ apm link
```
## JQuery

### [jqa] jQuery.ajax()

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

### [jqe] jQuery.fn.extend()

```javascript
$.fn.extend({
    ${1:methodName}: function (${2:options}) {
        ${3://body...}
    }
});
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Based on [Javascript Snippets for Atom](https://github.com/zenorocha/atom-javascript-snippets) by Zeno Rocha
