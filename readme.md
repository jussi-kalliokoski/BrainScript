BrainScript
===========

BrainScript is a scripting language that is a subset of JavaScript and inspired by Urban Müller's brainfuck.
Valid BrainScript is always also (syntax-wise) valid JavaScript, so all rules that apply to JavaScript, apply to BrainScript.
BrainScript – however – has some extra rules of it's own, BrainScript does not support String literals, comments, whitespace (except \n), Numbers or any use of alphanumerals.
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
Do note that the example will only work in Chrome, and older versions of Firefox.

Other
-----

 * [CodeExpression.js](https://github.com/jussi-kalliokoski/CodeExpression.js) supports BrainScript parsing.
 * [brainfuck](http://www.esolangs.org/wiki/Brainfuck) on [esolangs.org](http://www.esolangs.org).