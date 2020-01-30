# Perl

Perl is a general-purpose programming language originally developed for text manipulation and now used for a wide range of tasks including system administration, web development, network programming, GUI development, and more.

Perl, implemented in the C language, was originally developed by Larry Wall in 1987 as a general-purpose Unix scripting language to make report processing easier. Since then, it has undergone many changes and revisions. Currently it is in th version 5.30.1.

The language grew from its niche as a tool for system administrators who needed something more powerful than shell scripting and easier to use than C programming into a general-purpose programming language. Perl has a solid history of pragmatism and, in recent years, a disciplined approach to enhancement and backwards compatibility.

The Perl language is a combination of several individual pieces. Although spoken languages use nuance and tone of voice and intuition to communicate across gaps in knowledge and understanding, computers and source code require precision. You can write effective Perl code without knowing every detail of every language feature, but you must understand how they work together to write Perl code well.

It has been nicknamed "the Swiss Army chainsaw of scripting languages" because of its flexibility and power. In 1998, it was also referred to as the "duct tape that holds the Internet together," in reference to its ubiquitous use as a glue language.

Perl has a motto: There's more than one way to do it (TMTOWTDI or TIMTOWTDI, pronounced Tim Toady). The language was designed with this idea in mind, in that it “doesn't try to tell the programmer how to program.” As proponents of this motto argue, this philosophy makes it easy to write concise statements.

In this work the word *perl* should mean the executable program, the compiler, and *Perl* should mean the Language.

## Perl Philosophy

Perl gets things done.
> it's flexible, forgiving, and malleable. 

Capable programmers use it every day for everything from oneliners and one-off automations to multi-year, multi-programmer projects.  

Perl is pragmatic. You're in charge. You decide how to solve your problems and Perl will mold itself to do what you mean, with little frustration and no ceremony.  

Perl will grow with you. Here you'll learn enough to write real, useful programs and you'll understand how the language works and why it works as it does. 

Perl mongers takes advantage of this knowledge and the combined experience of the global Perl community to help you write working, maintainable code. 

### Expressivity

In computer science, the expressive power (also called expressiveness or expressivity) of a language is the breadth of ideas that can be represented and communicated in that language. The more expressive a language is, the greater the variety and quantity of ideas it can be used to represent.

Before Larry Wall created Perl, he studied linguistics. Unlike other programming languages designed around a mathematical notion, Perl's design emulates how people communicate with people. This gives you the freedom to write programs depending on your current needs. You may write simple, straightforward code or combine many small pieces into larger programs. You may select from multiple design paradigms, and you may eschew or embrace advanced features.

Learning Perl is like learning any spoken language. You'll learn a few words, then string together sentences, and then enjoy simple conversations. Mastery comes from practice of both reading and writing code. You don't have to understand every detail of Perl to be productive, but the principles in this chapter are essential to your growth as a programmer.

Other languages may claim that there should be only one best way to solve any problem. Perl allows you to decide what's most readable, most useful, most appealing, or most fun.  This expressivity allows master craftworkers to create amazing programs but also allows the unwary to make messes. You'll develop your own sense of good taste with experience. Express yourself, but be mindful of readability and maintainability, especially for those who come after you.

Perl novices often find certain syntactic constructs opaque. These idioms offer great power to experienced programmers, but it's okay to avoid them until you're comfortable with them.  As another design goal, Perl tries to avoid surprising experienced Perl programmers. For example, adding two variables (*$first_num + $second_num*) is obviously a numeric operation. You've expressed your intent to treat the values of those variables as numbers by using a numeric operator. Perl happily does so. No matter the contents of *$first_num* and *$second_num*, Perl will coerce them to numeric values.

Perl adepts often call this principle DWIM, or *do what I mean*. You could just as well call this the principle of least astonishment.

Given a cursory understanding of Perl, it should be possible to understand the intent of an unfamiliar Perl expression. You will develop this skill as you learn Perl

Popular saying among Perl hackers is *"Only perl can parse Perl"*. In its efforts to DWYM and provide a high level of expressiveness, Perl syntax is hideously contorted. A bareword might be a string, even with the *use strict* pragma. Perl's reserved words have their own special syntax, and user-defined subs with a prototype, defined at compile time, can similarly direct parsing.

Any character can be a delimiter if you pick your own delimiters, except some behave differently.

With syntax that starts off tricky, but then changes with the program, it's a miracle that even perl can parse Perl. So it's small wonder that the advice to anyone wishing to parse Perl in some utility is advised that only perl can parse Perl. The problem is that such a parse is necessary in order to write good indenters, cross referencers, syntax highlighting program editors, style checkers and the like.


## Perl Documentation

* Perldoc
* CPAN

## Perl Names

Names (or identifiers) are everywhere in Perl programs: you choose them for variables, functions, packages, classes, and even filehandles. Valid Perl names all begin with a letter or an underscore and may optionally include any combination of letters, numbers, and underscores. When the utf8 pragma (Unicode and Strings, pp. 19) is in effect, you may use any UTF-8 word characters in identifiers. These are valid Perl identifiers:

```perl
my $name;
my @_private_names;
my %Names_to_Addresses;
sub anAwkwardName3;
# with use utf8; enabled
package Ingy::Döt::Net;
```

These are invalid Perl identifiers:

```perl
my $invalid name; # space is invalid
my @3; # cannot start with number
my %~flags; # symbols invalid in name
package a-lisp-style-name;
```

Names exist primarily for your benefit as a programmer. These rules apply only to literal names which appear in your source code, such as sub fetch_pie or my $waffleiron.
Only Perl's parser enforces the rules about identifier names. You may also refer to entities with names generated at runtime
or provided as input to a program. These symbolic lookups provide flexibility at the expense of safety. Invoking functions or
methods indirectly or looking up symbols in a namespace lets you bypass Perl's parser. Symbolic lookups can produce confusing
code. As Mark Jason Dominus recommends1
, prefer a hash (Hashes, pp. 43) or nested data structure (Nested Data Structures,
pp. 58) over variables named, for example, $recipe1, $recipe2, and so on.

## Perl Data Types

Perl is a loosely typed language and there is no need to specify a type for your data while using in your program. The Perl interpreter will choose the type based on the context of the data itself.

Perl has three basic data types: scalars, arrays of scalars, and hashes of scalars, also known as associative arrays. Here is a little detail about these data types.


- [scalar][type-perl-scalar]
- [array][type-perl-array]
- [hash][type-perl-hash]

## Perl Modules

## Perl Idioms

### Context

### Implicit ideas

### 

# Global concepts for languages

Perl has a very diferent notion of sintax and expressiveness, so some concepts, considered global for other languages, will have different meanings for Perl. Below is a list of Global concepts accepted by Perl in a similar way than other languages do.

## Global Objects (not "types")

- [`Array`][global-object-array]
- [`Boolean`][global-object-boolean]
- [`Function`][global-object-function]
- [`Object`][global-object-object]
- [`RegExp`][global-object-regexp]
- [`String`][global-object-string]
- [`Map`][global-object-map]
- ...and [others][concept-global-objects]


[type-array]: ../../types/array.md



[global-object-array]: ./objects/array.md
[global-object-boolean]: ./objects/boolean.md
[global-object-bigint]: ./objects/bigint.md
[global-object-date]: ./objects/date.md
[global-object-error]: ./objects/error.md
[global-object-function]: ./objects/function.md
[global-object-json]: ./objects/json.md
[global-object-map]: ./objects/map.md
[global-object-math]: ./objects/math.md
[global-object-number]: ./objects/number.md
[global-object-object]: ./objects/object.md
[global-object-promise]: ./objects/promise.md
[global-object-regexp]: ./objects/regexp.md
[global-object-set]: ./objects/set.md
[global-object-string]: ./objects/string.md
[global-object-symbol]: ./objects/symbol.md
[global-object-typed-array]: ./objects/typed-array.md
[global-object-weakmap]: ./objects/weakmap.md
[global-object-weakset]: ./objects/weakset.md

## Object-oriented concepts

- [Classes][concept-classes]
- [Composition][concept-composition]
- [Encapsulation][concept-encapsulation] (see also [anonymous functions][concept-anonymous-functions] and [scope][concept-scope])
- [Inheritance][concept-inheritance] (see also [prototype-based inheritance][concept-prototype-inheritance])
- [Mutation][concept-mutation]
- [Objects][concept-objects] (see also [global objects][concept-global-objects])
- [Polymorphism][concept-polymorphism] (see also [duck-typing][concept-duck-typing])
- [State][concept-state]

[concept-classes]: ../../concepts/classes.md
[concept-composition]: ../../concepts/composition.md
[concept-encapsulation]: ../../concepts/encapsulation.md
[concept-inheritance]: ../../concepts/inheritance.md
[concept-mutation]: ../../concepts/mutation.md
[concept-objects]: ../../concepts/objects.md
[concept-polymorphism]: ../../concepts/polymorphism.md
[concept-state]: ../../concepts/state.md

## Functional concepts

- [Anonymous functions][concept-anonymous-functions]
- [Higher-order functions][concept-higher-order-functions]
- [Immutability][concept-immutable] (of primitives, and using `Object.freeze`)
- [Nested functions][concept-nested-functions]
- [Partial application][concept-partial-application]
- [Pure functions][concept-pure-functions]
- [Recursion][concept-recursion]
- [Type inference][concept-type-inference]

[concept-anonymous-functions]: ../../concepts/anonymous_functions.md
[concept-higher-order-functions]: ../../concepts/higher_order_functions.md
[concept-immutable]: ../../concepts/immutability.md
[concept-nested-functions]: ../../concepts/nested_functions.md
[concept-partial-application]: ../../concepts/partial_application.md
[concept-pure-functions]: ../../concepts/pure_functions.md
[concept-recursion]: ../../concepts/recursion.md
[concept-type-inference]: ../../concepts/type_inference.md

## General concepts

- [Arithmetic][concept-arithmetic]
- [Bitwise manipulation][concept-bitwise-manipulation]
- [Boolean logic][concept-boolean-logic] (see also [jsdoc][platforms-jsdoc])
- [Comments][concept-comments]
- [Conditionals][concept-conditionals]
- [Destructuring][concept-destructuring] (see also [destructuring assignment][concept-destructuring-assignment])
- [Duck typing][concept-duck-typing]
- [Enumeration][concept-enumeration]
- [Functions][concept-functions]
- [Loops][concept-loops]
- [Methods][concept-methods]
- [Rest parameters][concept-rest-parameters]
- [Scope][concept-scope]
- [Type casting][concept-type-casting] (see also [type inference][concept-type-inference])
- [Variables][concept-variables]

[concept-arithmetic]: ../../concepts/arithmetic.md
[concept-bitwise-manipulation]: ../../concepts/bitwise_manipulation.md
[concept-boolean-logic]: ../../concepts/boolean_logic.md
[concept-comments]: ../../concepts/comments.md
[concept-conditionals]: ../../concepts/conditionals.md
[concept-destructuring]: ../../concepts/destructuring.md
[concept-destructuring-assignment]: ../../concepts/destructuring_assignment.md
[concept-duck-typing]: ../../concepts/duck_typing.md
[concept-enumeration]: ../../concepts/enumeration.md
[concept-functions]: ../../concepts/functions.md
[concept-loops]: ../../concepts/loops.md
[concept-methods]: ../../concepts/methods.md
[concept-rest-parameters]: ../../concepts/rest_parameters.md
[concept-scope]: ../../concepts/scope.md
[concept-type-casting]: ../../concepts/type_casting.md
[concept-variables]: ../../concepts/variables.md

## Language specific concepts

- [`async`][keyword-async]/[`await`][keyword-await] [concurrency][concept-concurrency] model
- Arguments
  - All arguments are optional
  - Named arguments via [destructuring][concept-destructuring]
- [Event loop][concept-event-loop] (see also: [Events][concept-events])
- [Generators][concept-generators]
- [Hoisting][concept-hoisting]
- [Iterators][concept-iterators]
- [Modules][concept-modules] ([`import`][keyword-import], [`require`][keyword-require])
- Package Management
- [Prototype based inheritance][concept-prototype-inheritance]
- [Sameness][concept-sameness]
- [Strict mode][concept-strict-mode]
- [Typed arrays][global-object-typed-array]
- Types vs. objects (see also [prototype-based inheritance][concept-prototype-inheritance])
  - [Global objects][concept-global-objects]
  - [Arrays are objects, with indexer][global-object-array]
  - [Functions are callable objects][global-object-function]

[concept-concurrency]: ../../concepts/concurrency.md
[concept-events]: ../../languages/javascript/info/events.md
[concept-event-loop]: ../../languages/javascript/info/event_loop.md
[concept-generators]: ../../languages/javascript/info/generators.md
[concept-global-objects]: ../../languages/javascript/info/global_objects.md
[concept-hoisting]: ../../languages/javascript/info/hoisting.md
[concept-iterators]: ../../languages/javascript/info/iterators.md
[concept-modules]: ../../languages/javascript/info/modules.md
[concept-prototype-inheritance]: ../../languages/javascript/info/prototype_inheritance.md
[concept-sameness]: ../../languages/javascript/info/sameness.md
[concept-strict-mode]: ../../languages/javascript/info/strict_mode.md
[keyword-async]: ./keywords/async.md
[keyword-await]: ./keywords/await.md
[keyword-new]: ./keywords/new.md
[keyword-import]: ./keywords/import.md
[keyword-instanceof]: ./keywords/instanceof.md
[keyword-require]: ./keywords/require.md
[keyword-typeof]: ./keywords/typeof.md
[platforms-jsdoc]: ../../tooling/jsdoc.md

## Other important/interesting things

- Perl IDE
- The Perl VM
- Perl Web frameworks
- Perl Data frameworks
- Perl Math frameworks
- Perl bindings with C and other languages
- Perl as a shell script alternative

### user-land concepts

- Stream based programming (rxjs, observable -> might make it into language)
- Declarative programming (Vue, React etc)
- Transpilers (Babel, Buble, TypeScript, etc) -> corejs compatibility etc.
- Bundlers (Parcel, Webpack, Rollup, etc)
