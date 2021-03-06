[![Build Status](https://travis-ci.org/Copilot-Language/copilot-cbmc.svg?branch=master)](https://travis-ci.org/Copilot-Language/copilot-cbmc)

Overview
========
[copilot-cbmc](http://hackage.haskell.org/package/copilot-cbmc) A tool to
generate a driver using CBMC, a third-party tool (see Dependencies below) that
proves that the code generated by different C back-ends is equivalent.
Currently, this includes the C99 back-end and the SBV back-end.

Copilot is a stream (i.e., infinite lists) domain-specific language (DSL) in
Haskell that compiles into embedded C.  Copilot is similar in spirit to
languages like Lustre.  Copilot contains an interpreter, multiple back-end
compilers, and other verification tools.

Examples
=========
Please see the files under the Examples directory in the
[Copilot](http://hackage.haskell.org/package/copilot) for a number of examples
showing the syntax, use of libraries, and use of the interpreter and back-ends.
The examples is the best way to start.

Installation
============
The Copilot library is cabalized. Assuming you have cabal and the GHC compiler
installed (the [Haskell Platform](http://hackage.haskell.org/platform/) is the
easiest way to obtain these), it should merely be a matter of running 
     
         cabal install copilot-cbmc

However, we strongly recommend you install Copilot, which installs copilot-c99
and other packages automatically.  Execute

         cabal install copilot

Dependencies
=============
copilot-cbmc depends on the C model-checker, CBMC.
[CBMC](http://www.cprover.org/cbmc/) is a bounded model-checker for C code.  We
use CBMC to prove that two back-ends generating C generate semantically
equivalent C, to help detect bugs in C back-ends.

Resources
=========
[copilot-cbmc](http://hackage.haskell.org/package/copilot-cbmc) is available on
Hackage.

**Sources** for each package are available on Github as well.  Just go to
[Github](github.com) and search for the package of interest.  Feel free to fork!

Copyright, License
==================
Copilot is distributed with the BSD3 license. The license file contains the
[BSD3](http://en.wikipedia.org/wiki/BSD_licenses) verbiage.

Thanks
======
We are grateful for NASA Contract NNL08AD13T to [Galois,
Inc](http://corp.galois.com/) and the [National Institute of
Aerospace](http://www.nianet.org/), which partially supported this work.
