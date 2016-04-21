
# Making our workspace

Go has a general notion of paths and where to find things. Go looks for things relative to the `$GOPATH` variable value.  While you can change this I've found it easier just to follow the flow of how Go expect things to work. Assuming your `$GOPATH` was set your `$HOME` directory you should find a folder called *src*. This is where go looks for packages to compile against. It is also where we'll put our own code.

Under *src* create a directory called *replweather*.  If you are in your home directory then you can do this by typing `mkdir -p $HOME/src/replweather` at the command prompt. Now change to this directory you've created.

To recap here's the commands all in order

```
  export GOPATH=$HOME
  cd
  mkdir -p $HOME/src/replweather
  cd $HOME/src/replweather
```

Now we're ready to start. 
