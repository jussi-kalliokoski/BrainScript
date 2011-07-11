BrainScript
===========

BrainScript is a scripting language that is a subset of JavaScript and inspired by Urban Müller's brainfuck.
Valid BrainScript is always also (syntax-wise) valid JavaScript, so all rules that apply to JavaScript, apply to BrainScript.
BrainScript – however – has some extra rules of its own, BrainScript does not support String literals, comments, whitespace (except \n), Numbers or any use of alphanumerals.
Only dollar ($) and underscore (_) characters are allowed to be used as identifiers.

Hello world in BrainScript
--------------------------

Pops out a modal box saying 'Hello world.'

```javascript

_=+!![];__=_+_;$_$=[][$=[![]]+[!![]]+{}
,$[_+__]+$[(__<<__)+__]+$[(__<<_)+__]+$
[(__<<_)+_]],$+=$_$,$_$=$_$(),$+=$_$+(+
{})+(_/(+!{})),$+=($[$$=$[(__<<_<<__)-
__]+$[(__<<__)+__]+$[(__<<__<<__)-(__
<<_)-__]+$[__+_]+$[(__<<_)+_]+$[(__<<_)
+__]+$[(__<<__)-_]+$[(__<<_<<__)-__]+$[
(__<<_)+_]+$[(__<<__)+__]+$[(__<<_)+__]
])+(+!![])[$$],$+=($_=$_$[$[(__<<__<<__
<<_)-(__*__)-(__<<__)]+$[(__<<__)+__]+$
[(__<<_<<__)-__]+$[(__<<__)-_]+$[(__<<
__<<__<<__)+__*__]+$[__<<_]+$[(__<<__<<
__)-(__<<_)-__]+$[(__<<_)+_]])+(_/__),
$_$[$[_]+$[__]+$[__<<_]+$[(__<<_)+__]+$
[(__<<_)+_]]($[(__<<__<<__<<__)+(__<<__
<<__)+(__<<_)]+$[__<<_]+$[__]+$[__]+$[(
__<<__)+__]+$[__<<__<<_]+$[(__<<__<<__
<<_)+(__<<__)+_]+$[(__<<__)+__]+$[(__<<
_)+__]+$[__]+$[(__<<__<<__<<_)-(__*__)-
(__<<__)]+$[(__<<__<<__<<__)+(__<<__<<
__)+(__<<__<<_)+__]);

```

The JavaScript equivalent would be

```javascript

alert('Hello world.');

```
Do note that the example will only work in Chrome and older versions of Firefox.

Compiling
---------

The compiler folder inludes a JavaScript -> BrainScript compiler for whatever purposes you may have for such a thing. Currently known issues are bloated size (this is not noticeable when gzipped) and memory usage. Also, it introduces some public variables, but just put all your javascript in a single file and compile, and you should be all right!

Like any credible language, BrainScript also features a compiler written in BrainScript, you can find it in ``` compiler/self-compiler.html ``` .

The proper MIME type for BrainScript is ``` text/x.brain+javascript ```. It however works with ``` text/javascript ``` as well.

Pros
----

 * Easy to understand, simple syntax. Should be familiar to most of the people, as it's the same as in the world's most popular programming language.
 * Very high gzip compression ratio (usually around 98%).
 * Hard to do dangerous or 'evil' things with.
 * There's nothing to get in the way of you and the desired result, when there are no keywords, literal control structures or other useless things.
 * Everything you could do with JavaScript, you should (be able to) do with BrainScript.
 * Makes debugging more enjoyable.
 * Allows you to exceed the charset of your BS file.
 * The syntax is understood by all browsers that support JavaScript.

Deltas
------

 * Writing X-Browser compatible code isn't always – well... – possible. Implementations are getting better though.
 * Introduces some "global pollution".
 * The current compiler introduces some (massive) memory leaks to your code. Working on it.
 * Firefox 5+ doesn't support BrainScript. Older versions, however, do.

Other
-----

 * [CodeExpression.js](https://github.com/jussi-kalliokoski/CodeExpression.js) supports BrainScript parsing.
 * [brainfuck](http://www.esolangs.org/wiki/Brainfuck) on [esolangs.org](http://www.esolangs.org).
 * [JavaScript specification](http://www.ecma-international.org/publications/standards/Ecma-262.htm) or [EcmaScript 5th edition](http://es5.github.com/) (There's some dispute whether or not BrainScript is compatible with ES5)

Authors
-------
 * [Juha Halme](https://github.com/juha-halme/)
 * [Jussi Kalliokoski](https://github.com/jussi-kalliokoski/)
