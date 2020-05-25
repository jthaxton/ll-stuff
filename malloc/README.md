# ll-stuff

## Strategy
We are using a linked list of header type structs that contain blocks of memory that can either be free or not. Each block is aligned on 16 bytes.

## How to run
```bash
$ ./run.sh
```

But if you want to compile then run individually, use
```bash
$ gcc memory.c
```
then 
```bash
$ ./a.out
```

If you want to autoload these functions into your c code, you can also use

```bash
$ gcc -o a.so -fPIC -shared memory.c
$ ~/.bashrc << export LD_PRELOAD=$PWD/a.so
```

