@def title = "JuDoc Sandbox"
@def hasmath = false
@def hascode = false


# Jekyll

* [2012-03-11-shelling-out-sucks](pub/2012-03-11-shelling-out-sucks.html)
* [2013-05-10-callback](pub/2013-05-10-callback.html)
* [2013-04-05-distributed-numerical-optimization](pub/2013-04-05-distributed-numerical-optimization.html)

## Notes

### Easy fix

### Medium fix

### Could be automated

* internal link convention is different (see fixes in _shelling out sucks_ could find and replace occurences of `(#...)` by lowering and using `_` instead of `+` and that would fix most of the stuff)
* `\\(` to `$`  and `\\)` to `$`

### Other notes

* lists: need things on the same line (see issue [#213](https://github.com/tlienart/JuDoc.jl/issues/213))
* date and author not shown at the top (this is layout stuff so not a bug)
* is strike through a convention? --> doesn't seem like it is
* direct inclusion of html is not ok, need triple tildes
