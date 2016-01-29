# zvm

A minimal register-based virtual machine in zepto.

## Usage

This virtual machine takes a minimal, assembler-esque
language, compiles it to byte-code and runs it on a
register machine.
An example script can be found in the `examples/` dir.

The result of all the opcodes are saved in the first register
specified.
The opcodes that are understood are 
- noop: does nothing
- add: adds two registers
- sub: substracts two registers
- mul: multiplies two registers
- div: divide two registers from each other
- print: print the contents of one register
- and: bitwise and on two registers
- or: bitwise or on two registers
- not: bitwise negation of a register

I made sure no useful programming is possible.

If you want to try it out and have zepto installed
(*why would you have that?*), you can just run:

```sh
zepto vm-cli.zp somevmfile
```

## Why

Simple: Because I've never written a register-based
virtual machine before and I wanted to try it out.

<hr/>

Have fun!
