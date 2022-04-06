# GHW Share | Hello-World-in-FreakC
A new esolang to dive into.


## What is FreakC, you ask? 

`print[] Hello, World.`

FreakC is a nice, little, multi-paradigm programming language, which looks like Batch, compiles to Batch and is written in Batch as well. It is mainly built to be an experimental project with the idea of creating a programming language in such a limited language like Batch, but then it turns out that FreakC has added a little bit of features to Batch that might come in handy for some Batch developers. Batch's commands should work with FreakC most of the time, however, there are some quirks you should consider checking out which I have mentioned in the next part of this document.

And yes, this is not a C dialect, it's more like C in ArnoldC.

FreakC's commands end with [] or a special operator to indicate that it's FreakC code, so it doesn't cause confusion with Batch codes in your code.

## How is FreakC any different from Batch? 

**FreakC's added features compared to Batch:**

- While loops, repeat-until loops, and FreakC's own for loops with break/continue supports.

- Switch cases.

- Class-based OOP.

- A bunch of utility functions for you to use.

- Inline functions.

- Macros.

- Some minimal operators.

- Floating-point numbers.

- Some additional commands.


## Hello World in FreakC

• Hello World, normally:

```
print[] Hello, World!
```

• Hello World using function:

```
function[] SayHelloWorld

    print[] Hello, World!

endfunc[]

:: Calling "SayHelloWorld" function, printing out "Hello"

SayHelloWorld[..]

:: This will also work, because Batch's commands work in FreakC:

call SayHelloWorld
```

Note: `::` are used to provide comment lines.

## Resources:

[FreakC's official GitHub Page](https://github.com/FreakC-Foundation/FreakC)


## Switching from Batch to FreakC

While FreakC is compatible with Batch, but it's not 100% compatible, you just need to replace all `!` with `^!`, `^^!` with `^^^^^!` (the second one is only required in enabled delayed expansion). If you use codes that depends on blank lines, then just change them to the `!` character to create a blank line entirely, or just use Batch's `^`.
