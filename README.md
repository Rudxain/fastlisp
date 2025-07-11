# fastlisp
fastlisp is an easiness oriented reduced scripting language. an easiness oriented programming language makes most (if not all) of its design decisions to try to make the language easier to teach, learn, use, and extend. One approach to attain easiness is by taking a scripting language that is already easy and reducing its complexity.

fastlisp takes the semantical essence of lisp and reduces it down to a system small enough to fit into the **boot sector of a floppy disc**. it is designed to be compatible with
_sectorlisp_. its specification fits into a qr-code. because of its extremely small size, it is trivial to memorize the operation of the **entire** language. this memorization allows the user's knowledge of the language to crystalize earlier on in the process of development, and the goal is that this will help to give it a competitive advantage over traditional lisps in the _"easy languages"_ category.

fastlisp is easy because of its architecture. it comes with two parts:
1. its **base**, which is the [lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus). any abstract machine could act as its base, but lambda calculus is suited for a lisp syntax, and lambda calculus is also trivial to teach.
2. its **notation** for writing and recommended style, which provides a lisp-like set of semantics. the lisp style of writing with [s-expressions](https://en.wikipedia.org/wiki/S-expression) is a universal way to express a given algorithm, and once one knows what algorithm is to be implemented, it is easy to guess what that algorithm might look like in lisp. It is a universal set of semantics that can express any algorithm with the same set of rules. This prevents the user from having to continually learn new syntaxes, semantics, and grammars, in order to operate the base language.

fastlisp is much like a sea creature with only one hole for both eating and defecating. fastlisp takes an input program, it calculates the value of that input program, and it returns an output program. it performs this operation once then halts forever. although it [isn't guaranteed to halt](https://en.wikipedia.org/wiki/Halting_problem), there are sub-sets of fastlisp that are guaranteed to halt. in order for fastlisp to continue computation, it must be restarted by an outside program with a new fastlisp program to compute; therefore, fastlisp systems take a programs as input, processes them, then output programs. fastlisp systems are orchestrated by external systems that aren't fastlisp.

fastlisp is capable of scripting language performance, and is suitable for writing libraries that help to generate code in other languages. it is recommended to the user that they use fastlisp to generate code in python for both high-level and low-level tasks. fastlisp makes the process of generating code in other languages (such as python) trivial. one can be programming in what is called _telestial_ fastlisp, while unaware that their code is describing actions in python under the hood. by generating python, more high-performance computing is possible.

fastlisp came pre-equipped with the ability to _absorb_ nearly all of the immutable code base from the haskell programming language, because the haskell system can be dumped right into a lambda. it should be noted that the nix community had made it against the rules to discuss the topic of dumping the nix language into a lambda, which is a very closed-minded way of operating. fastlisp is also capable of _"stealing"_ much of the code written in python by being used to generate python. it is trivial to take a python library and turn it into a usable fastlisp library with ordinary fastlisp library functions as the interface. thus with its own library of immutable code compatible with pure fastlisp, and the ability to generate code that takes advantage of any exiting or future python code, it is trivial to populate fastlisp with diverse and performant code.

some might say "fastlisp is just an abstraction on python. fastlisp is just an abstraction in general." it is a common misconception and meme among college graduates that abstraction is useless.

fastlisp supports a wide range of programming styles because its syntax is _nearly_ _completely_ _reprogrammable_. Not only is its base syntax extensible and semantically powerful, but it has the ability to have its syntax extended arbitrarily thus adopting notations from any other language such as the notation of working queries from sql, or the notation of linq from c#, or the notation of prolog. this means of extending the syntax via macros has traditionally been considered too dangerous to use, even by the military. fastlisp considers the user's semantical freedom paramount, and does not compromise in this area.

fastlisp is based on some of the combinatorial work originally done by moses schonfinkle, who was a fan of hilbert. fastlisp is an attempt at reductionist computing in a hilbert fashion, with the radical take that mathematical consistency is less desirable than mathematical completeness for computer systems. not only is the ability to write proofs irrelevant for most computer programming, but a programming system *must* be able to simulate *any* system with *any* *set* *of* *axioms*. in order to simulate any system with any axioms, an inconsistent system is necessary at the base. this approach vindicates hilbert and makes his goals seem once again attainable. future versions of the fastlisp style of language architecture are hoped by it's creator to be a successful attempt at something like russel's principia mathematica in consuming all of mathematics with one universal system.

what differentiates fastlisp from combinatorics lambda calculus, lisp1, and sector lisp is that fastlisp has is an easier notation for lambdas with the notion of strings that are sugar for lambdas. this means that the notion of integers, floating point numbers, booleans, binary data, hex data, strings, and all manner of other data may be concisely expressed as strings. this is the semantical power that something like sector lisp lacks. it is designed to be compatible with sector lisp so that sector lisp can be extended to have this expressive power (i'm looking at you, jart).

it is recommended that the user of fastlisp use these combinators: the ibis, the kestrel, the kite, the viero, and the z. the ibis may serve as if and lisp's quote. the kestrel may serve as the boolean true, as the logical or, and as the lisp function car. the kite may serve as the boolean false, as the logical and, and as the lisp function cdr. the kestrel and kite can be combined to form the not function thus allowing for nand, and nor. the viero allows for the creation of linked lists and binary search trees, and is essentially lisp's cons. combinations of ibis, kestrel, kite, and viero, when used properly, should always halt, and should always be finite but may self contradict. the z combinator allows for recursion and each recursion allows for the passing of one object back to the beginning of a function.

The combination of ibis, kestrel, kite, viero, and z, should allow for a general purpose set of primitives that can be used to bootstrap the rest of the functionality that one might expect from lisp when combined with macros. This combinatorial approach is what was proposed by shonfinkle.

The lambda can be defined as a function that takes a name and takes a definition and defines a program in an environment where that definition is synonymous with that name. So if we want to create an environment where the ibis exists, and call it up on itself twice, then we might say `(lambda ibis (ibis ibis ibs))(lambda x x)`. This is how let or define is performed in the lambda calculus, and is the primary mode of function abstraction.

fastlisp is inspired in part by JSON and intends to be a turing-complete replacement for JSON. Part of the design of fastlisp is for it to be easily implementable like how JSON is so that it can spread ubiquitously about software stacks.

fastlisp is embeddable almost directly into any language that has lambdas, and requires only a couple of regular expressions to be made compatible with some mainstream languages. By converting it to the right lambda expression it can be embedded directly into: python, f#, typescript, javascript, ocaml, scala, common lisp, scheme, kotlin, and many more languages. This embeddability means that fastlisp is able to go where no language has gone before.

fastlisp is designed for both the lowest denominator of programmer and the highest denominator of programmer in terms of skill and ability. fastlisp is designed to be as easy as possible so a 14 year old who is not inclined to math could learn it in a short time, ideally during 1-7 classroom sessions. It is also designed with military jar heads in mind who may need to be taught something quickly so that they can be effective in programming fast. It is designed with art students in mind who do not want to memorize lots of inane details and functionality about a programming language merely in order to implement algorithms. fastlisp leaves little room for the learner to misunderstand how the language works. This scarcity of ambiguity about fastlisp leaves little to be desired in terms of teachability and learnability. One does not have to wonder "do I know enough code to write any algorithm I want." With fastlisp they can rest in the knowledge that they have quickly and completely memorized a syntax that is indeed powerful enough to program anything that they should like to program.

fastlisp is designed with engineers in mind as well as beginner programmers. fastlisp aims to offer an interface for engineers to talk abstractly and in a high level way about an algorithm that they want. Through library abstraction code generation tools can be built to help, with the aid of the human, generate similar kinds of machine code as languages like fortran, c, c++, and rust. Although the ability to generate code in python is sufficient for most tasks, libraries can be created in fastlisp for the user to not only generate code in a low level language, but optimize it and go over the finer details of what is to happen on the machine. This ability to use libraries that allow for fine tuned performance controls is what allows the human to achieve the same manual hand-coded optimizations as are available in c++. For anything that is not absolutely performance critical, generating program that takes advantage of the speed and libraries of python should be trivial and time-saving for an engineer.

It should be noted that lambda calculus may not be suitable for the core of fastlisp. If this turns out to be true, another similar language will be created with a different abstract system, such as the category theory. In all likelihood it would be a system that abstractly incorporates the ideas of arrays and integers.

fastlisp is not mathematically consistent but it can be used to generate libraries that allow for the control of consistent systems bound by proof checkers.

fastlisp does not have a type system but it allows for the creation of any desired type system. fastlisp does not have the ability to force this type system on the user, however it may be possible to make systems where those systems cannot be interacted with without using said type system or poking memory, thus creating an enforcement of type safety.

With the z-combinator fastlisp is able to recurse in a strictly typed language without necessarily stack overflowing.

It is suggested to the user that text in fastlisp be sugar for lists of booleans, because this is the most data dense data-structure that fastlisp is currently known to be able to host to encode strings. There may be a more data dense method that can be found in binary lambda calculus. Ideally the most data dense possible format should be used to encode strings in fastlisp.

In fastlisp text is meant to encode ints, big ints, floats, big floats, strings, hex data, and essentially anything that isn't a function name.

fastlisp on its own is capable of `eval` if the `eval` has no awareness of anything that was previously defined. However with macros or with other techniques it is possible to create an `eval` that is contextually aware of what is currently defined.

The forwards and backwards compatibility of fastlisp has been deeply considered. fastlisp should by design run the same way until the end of time except for evaluation order. fastlisp should be a stateless design that never in theory needs to be updated. Furthermore it should be trivially compatible with other similar systems along the same design philosophy. fastlisp is designed from the ground up to be able to run on some of the oldest computers and all future computers. fastlisp is designed to be able to run on any operating system and to be made compatible for any software for which it is possible to be made compatible in as easy a manner as is possible.

fastlisp is licensed to be able to be used in both commercial and in open source endeavors, it has a permissive license that insists the lack of liability of the author should some fool choose to use such a system. fastlisp indeed comes with no warranty of merchantability or fitness. that being said people may make closed source and open source programs and standards with fastlisp.

fastlisp is not only an immutable specification for a language, but it is an immutable language. This means that while the program is running it is stateless but could be used to simulate state. This means that some multicore paralellism or concurrency can be gained partially for free by passing fastlisp into the right kind of system (such as [hvm](https://github.com/HigherOrderCO/HVM)).

fastlisp may not be the first successful language of its kind, but it is a unique first-of-its-kind language that takes existing software off of the shelf and utilizes it in a novel way.

every fastlisp program is a stateless lambda expression. to compile to another language, merely express the program as a lambda in that language.

fastlisp has no debugger, or compiler messages/warnings/notes, but it is possible to implement these if needed.

generally in fastlisp it is good practice to return a list containing three things: the last working copy of the machine with all of its state, the output of the program, and optionally any instructions that the program wants the outside computer to carry out.

If a language is to be generated besides python, the official way to do this is to use fastlisp to generate python that generates code in that language. This hierarchy helps to simplify the fastlisp ecosystem.

If fastlisp is compiled to a lambda expression in another language like python, and that lambda takes as an input a function that is not a pure lambda, we are no longer talking about a fastlisp lambda. that is no longer a piece of runtime celestial fastlisp, it is a piece of python code. It still shares many of the properties of the fastlisp it once was, but technically it isn't fastlisp. fastlisp is composed of pure lambdas only.

things that are needed: 

* a program written in pure fastlisp that takes a fastlisp program as input and rewrites it as one long lambda in python
* some code that takes immutable code from haskell and dumps it into a fastlisp lambda
* a working version of awk written in pure fastlisp
* a fastlisp shell
* fastlisp documentation
* fastlisp guide for beginner programmers
* useful libraries in python that are absorbed into fastlisp telestial libraries

in fastlisp there are tiers of fastlisp code named after mormon heavens. subterranean code is code that is not fastlisp. terrestrial code is fastlisp code that directly generates code in another language. telestial fastlisp code is code that depends on terrestrial fastlisp code but where the user might not necessarily need to be aware that they aren't using pure fastlisp. instead, telestial code is ideally seamless with no obvious remnant of the language it depends on in the function interface. Finally, celestial fastlisp code or pure fastlisp code does not depend on any subterranean, terrestrial, or telestial fastlisp code. Only celestial fastlisp code is guaranteed to run the same way until the end of time except for evaluation order.

All fastlisp code depends on subterranean code to run and operate. However that subterranean code can be generated with fastlisp.

Ideally one day the dependency of python will be removed from the majority of fastlisp codebases.

fastlisp does not have an object or class system but it is trivial to add one.

the fastlisp compiler for now is called `fastlisp-to-python-compiler.py`. It takes a fastlisp program from `stdin` and returns a python lambda to `stdout`. `fastlispsamplecode.fastlisp` is a file that contains a fastlisp program with an environment with useful functions preprogrammed into it.

For info about fastlisp email me at john.morris.beck@hotmail.com
