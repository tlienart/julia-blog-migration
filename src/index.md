@def title = "JuDoc Sandbox"
@def hasmath = false
@def hascode = true


# Jekyll

* [2012-03-11-shelling-out-sucks](pub/2012-03-11-shelling-out-sucks.html)
* [2013-05-10-callback](pub/2013-05-10-callback.html)
* [2013-04-05-distributed-numerical-optimization](pub/2013-04-05-distributed-numerical-optimization.html)
* [2017-11-01-gsoc-ode.md](pub/2017-11-01-gsoc-ode.html)
* [2019-09-07-julia-workshop-beijing-zh_cn](pub/2019-09-07-julia-workshop-beijing-zh_cn.html)

## Playground

* Dollar symbol, 1000\$, also 1000&#36;
* Backslash symbol, \ don't escape that one as that's a shortcut for a line return for instance:

`some text \\ then some text` becomes:

some text \\ then some text

### Comments from [@cormullion](https://github.com/cormullion), [issue #201](https://github.com/tlienart/JuDoc.jl/issues/201)

* (**done**) dollar signs &rarr; just escape the symbol in text like so: \$ other currencies are not affected £ € ¥
* (**done**) double backticks &rarr; are now supported like so ``this is ` in double`` etc.
* (**can be automated**) math issues &rarr; replacing `\\(...\\)` for `$...$` works
* (**done**) julia (and other) indented code like so:

    function foo()
        return 3
    end

    function bar()
        return foo() + 5
    end

* (**piping post**) see link above and `\n` are now handled properly: `here: \n and blah`
