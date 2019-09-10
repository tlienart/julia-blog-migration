# Readme

Experimental repo to migrate blog posts from Julia blog into [JuDoc](https://github.com/tlienart/JuDoc.jl) format.

The aim of the repo is to see what needs to be addressed when moving from julia-blog syntax (effectively Jekyll) to JuDoc.
The posts were selected more or less at random.

## How to "use" this repo

Assuming you have JuDoc, just clone this repo to your computer, `cd` to the folder and

```julia
using JuDoc
serve()
```

then navigate to `localhost:8000`.

## Notes

### Could be automated

* internal hyperref link convention is different (see fixes in _shelling out sucks_ could find and replace occurences of `(#...)` by lowering and using `_` instead of `+` and that would fix most of the stuff) so for instance

`*[Metacharacter brittleness.](#Metacharacter+Brittleness)*`

should be replaced by

`*[Metacharacter brittleness.](#metacharacter_brittleness)*`

* inline maths: effectively just change `\\(` to `$`  and `\\)` to `$`
* use of `$` symbol, basically just escape it `\$`

### Other notes

* lists: need things on the same line (see issue [#213](https://github.com/tlienart/JuDoc.jl/issues/213))
* date and author not shown at the top (this is layout stuff so not a bug)
* is strike through a convention? --> doesn't seem like it is
* direct inclusion of html is not ok, need triple tildes
* in JuDoc you (currently) need to specify the title twice, once with a `@def` (which will go to a `<title>` tag used in the tab name) and then in a top header `# title`; probably both can be done in once, see [issue #10](https://github.com/tlienart/JuDoc.jl/issues/10)
