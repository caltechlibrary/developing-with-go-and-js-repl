
# Developing with go and a JavaScript REPL

This is a demonstration of creating a simple middle-ware and JavaScript REPL based on [otto](https://github.com/robertkrimen/otto) JavaScript implementation, [ostdlib](https://github.com/caltechlibrary/ostdlib) and the [weather.gov REST API](http://graphical.weather.gov/xml/rest.php).  It assumes you're either following along verbatim or you've gone through the Go language tutorials at [golang.org](http://golang.org).

Why Go and a JavaScript REPL?  Well Go is fun, compiles reasonable fast but is not an interpreted dynamically typed language. JavaScript is an interpreted dynamically typed language.  I have found doing ad-hoc or exploratory coding to benefit from the immediate feedback and flexibility found in interpreted dynamically typed laugange. On the other hand when I want things to "just work" and be solid I like Go.  Fortunately Go and JavaScript lively happily together thanks to Robert Krimen's Go package named otto.

## table of contents

1. Before we begin
2. [setting-things-up.md](setting-things-up.md)
3. [replweather](https://github.com/rsdoiel/replweather) - an example implementation of what we will be creating
4. [making our workspace](making-our-workspace.md)
5. [hello world](helloworld.md)
  + If you're having problems at this point please checkout [golang.org](http://golang.org) and one of the excellent Go tutorials
6. [rw1](rw1.md) - a very simple JavaScript [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
7. [rw2](rw2.md) - a JavaScript REPL with some extensions from [ostdlib](https://github.com/caltechlibrary/ostdlib)
8. [rw3](rw3.md) - An initial JavaScript REPL with weather.gov RSS content


## Reference material

+ If you are new to go...
    + [Golang-book](http://www.golang-book.com/)
    + [Take a Tour](https://tour.golang.org/welcome/1)
    + Try the Golang Wiki/[learn](https://github.com/golang/go/wiki/Learn)
+ [weather.gov REST API](http://graphical.weather.gov/xml/rest.php)
    + [example xml](http://graphical.weather.gov/xml/DWMLgen/schema/latest_DWML.txt)
    + [format](http://graphical.weather.gov/xml/mdl/XML/Design/MDL_XML_Design.htm)
+ [ostdlib](https://github.com/caltechlibrary/ostdlib)
    + [otto](https://github.com/robertkrimen/otto)
    + [readline](https://github.com/chzyer/readline)
    + [xlsx](https://github.com/tealeg/xlsx)
    + [color](https://github.com/fatih/color)
+ [micro](https://github.com/zyedidia/micro)
