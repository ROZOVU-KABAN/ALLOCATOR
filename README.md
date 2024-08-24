gcc -o memalloc.so -fPIC -shared main.c

export LD_PRELOAD=$PWD/memalloc.so

unset LD_PRELOAD
