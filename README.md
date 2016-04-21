
# Developing with go and a JavaScript REPL

This is a demonstration of creating a simple middleware and JavaScript REPL based on [otto](https://github.com/robertkrimen/otto) JavaScript engine, [ostdlib](https://github.com/caltechlibrary/ostdlib) and the [weather.gov REST API](http://graphical.weather.gov/xml/rest.php).  It assumes you're either following along verbatum or you've gone through the Go language tutorials at [golang.org](http://golang.org).

Why Go and a JavaScript REPL?  Well Go is fun, compiles reasonable fast but is not an interpretted dynamically typed language. JavaScript is an interpretted dynamically typed language.  I have found doing ad-hoc or exploritory coding to benefit from the immediate feedback and flexibility found in interpreted dynamically typed lauange. On the otherhand when I want things to "just work" and be solid I like Go.  Fortunately Go and JavaScript lively happily together thanks to Robert Krimen's Go package named otto.

## table of contents

1. [setting-things-up.md](setting-things-up.md)
2. [making our workspace](making-our-workspace.md)
3. [hello world](hello-world.md)
  + If you're having problems at this point please checkout [golang.org](http://golang.org) and one of the excellent Go tutorials
4. [r1](r1.md) - making a very simple JavaScript [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
