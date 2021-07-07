# test-ode-drawstuff-on-mac
test the demo of ode together with drawstuff on my M1 Mac mini

## Install script 
```clang++ `pkg-config --cflags --libs ode drawstuff` -o myapp demo_basket.cpp```

When it has error like this:

ld: symbol(s) not found for architecture arm64
clang: error: linker command failed with exit code 1 (use -v to see invocation)

Undefined symbols for architecture arm64


## Then it is because you're using GCC(CC) or Clang!

**You should use Clang++ (or maybe g++)!**
