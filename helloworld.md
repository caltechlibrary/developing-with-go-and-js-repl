
# Hello world

This is the traditional first program in a new programming language. We're going to use it to make sure Go is setup as expected.
We need to do three things to get our compiled version of hello world.

1. Change to the project directory
2. Create an appropriately named subdirectory 
3. Type in our program (I'm assuming you're using the text editor called *micro* if not use your favorite text editor)
4. Run the build command 
5. See if it works

Here's what I've done specifically for *helloworld*.

```
  cd $HOME/src/replweather
  mkdir -p cmds/helloworld
  micro cmds/helloworld/helloworld.go
  go build cmds/helloworld/helloworld.go
  ./helloworld
```

When you run *helloworld* you should see the usually output. The text of *helloworld.go* should be as follows

```
  package main
  
  import "fmt"
  
  func main() {
    fmt.Println("Hello World!")
  }
```

Notice the redundant name for the directory and program. This is typical in Go projects.  Now we need to edit the *helloworld.go* file and
type in the source code to display our traditional message. Again feel free to replace *micro* for the text editor of your choice.

