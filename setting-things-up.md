
# Setting things up

You will need at a minimum two pieces of software-- git (for fetching the current version of Go) and Go. We can build the rest from packages (e.g. a simple text editor, otto, ostdlib). You will need access to the internet to fetch the files.

Git is a source code version system. You can find out more information about [git](https://git-scm.org) at the [git-scm.org](http://git-scm.org) website.

Go is a programming language originally developed at Google but now a fully open source language developed by the Go community.  It is a compiled langage well suited to working with web resources and building web services. If you don't have Go installed already please take a look at the [golang.org](http://golang.org) website. You'll want Go 1.6.x for this tutorial.

There are many text editors in the world.  While I don't recommend one editor over another the ones I commonly use today include vi, nano, and Atom. There is even a text editor for the terminal written in Go called [micro](https://github.com/zyedidia/micro) so in principle you could install Go then Micro and follow along with that.

## How I usually setup Go

I've been using Go a while and usually compile it from scratch. If you have your the usual C language toolchain installed on your Unix/Linux/Mac OS X box it is pretty straight forward.

1. Change to your home directory
  + `cd`
2. Clone the git repository for go as go1.4
  + `git clone https://github.com/golang/go go1.4`
2. Change directory to go1.4
  + `cd go1.4`
4. Checkout the git tag "go1.4.3"
  + `git checkout go1.4.3`
5. Change to the src directory and run *all.bash*
  + `cd src`
  + `./all.bash`
6. Change back to your home directory
  + `cd`
7. Clone the git repository for go to go
  + `git clone https://github.com/golang/go go`
8. Change directory to go
  + `cd go`
9. Checkout the the git tag go1.6.2
  + `git checkout go1.6.2`
10. Change to the src directory, run *all.bash* and return to your home directory
  + `cd src`
  + `./all.bash`
  + `cd`
11. Add go/bin to your path
  + `export PATH=$HOME/go/bin:$PATH`
12. Set $GOPATH environment variable
  + `export GOPATH=$HOME`

If all has gone well you should have a working Go compiler and tools installed in `$HOME/go/bin`.  

## Install additional Go packages

If you want a simple text editor then you can install zyedidia's [micro](https://github.com/zyedidia/micro) using the `go get` command.

```
  go get github.com/zyedidia/micro/...
```

Notice the trailing three dots. That's important to type. This tells the `go get` command to install not just the package files in your `$GOPATH/src` directory but also compile and install any commands found.

Now we need to install a number of packages that are required by this tutorial. We will be installing

+ github.com/robertkrimen/otto a JavaScript engine written in Go
+ github.com/chzyer/readline a readline package written in Go
+ github.com/tealeg/xlsx a package for working with Microsoft Workbook files (i.e. files ending in .xlsx)
+ github.com/fatih/color a package that lets you render color output in the terminal
+ github.com/caltechlibrary/ostdlib a wrapper library that combines the above for exposing a nice REPL with help, readline support and color options

All these packages get installed with the usual `go get` command.  Here's the list of command I have run

```shell
  go get github.com/robertkrimen/otto
  go get github.com/chzyer/readline
  go get github.com/tealeg/xlsx
  go get github.com/fatih/color
  go get github.com/caltechlibrary/ostdlib
```

Now we should be ready to start the tutorial!
