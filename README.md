# A whole lotta weasels

A joint effort to write the [Dawkins' Weasel algorithm][wikipedia] in as many languages as possible, using the language's specific idioms.

Algorithm described [here][algorithm].

+ Each implementation should only be one file and placed in the root folder.
+ Each file should be named by the language in which it was written.
+ The program should print the fittest string of each generation, as well as the number of generations it took.
+ Mutation rate should be 4%, generation size 100.


Each implementation should, as far as it is feasable, capture the charachteristics of that language. The goal is readable and enjoyable implementations in as many languages as possible.

[wikipedia]: http://en.wikipedia.org/wiki/Weasel_program
[algorithm]: http://rationalwiki.org/wiki/Dawkins_weasel

=======
# Building the examples:

Below are the basic instructions to run the code examples, sorted by OS -> Language.

## Ubuntu

### Python

    python python.py

### Haskell

    runhaskell haskell.hs

### Go

    apt-get install go
    go run go.go

### D

    apt-get install gdc
    gdc d.d
    ./a.out

### F&#35;
first install mono:

        apt-get install mono

clone the [github repo][fsharp-github] and follow the instructions there (make && make install)

then:

        fsharpc fsharp.fs
        mono fsharp.exe

[fsharp-github]: https://github.com/fsharp/fsharp

### Common Lisp
install:

    apt-get install sbcl

run:

    sbcl --script common-lisp.lisp

### Coffeescript

1. install node via apt-get
2. install coffee-script via npm
3. run:

        coffee coffee-script.coffee
		
		
### Nimrod

	1. Compile Nimrod from the github sources
	2. run:
	
		nimrod -r nimrod.nim

### perl

    perl perl.pl

### Visual Basic 6

1. Start Visual Basic 6
2. Select "Standard EXE" from the new projects dialog
3. Add "visual-basic-6.mod" to the project ("Add Module")
4. Double click on the form to enter `Form_Load()` event
5. Type `Call WeaselProgram` in the event
6. Hit F5 to run

Since VB6 is the base for VBScript, the VB6 weasel can easily be converted to VBScipt. For example  to run in Excel, create a new macro and replace `Debug.Print ` with `Range("A" & excel_row).Value = `, where `excel_row` is an incrementing variable for keeping track of the current row.


