# Sword

The PUC Lua interpretor seems not planned to be a batteries-included language (like python) and stay ANSI C compatible only.

```
  <TsT> cmtptr, do you know why there is not socket support maintained by the official Lua team ?
<cmtptr> TsT, lua is not intended to be a batteries-included language
<cmtptr> and sockets are not available in ANSI C
  <TsT> that's a shame :p
<cmtptr> no, I like it that way
 <rjek> If you want batteries, you know where Python is.
```


We will never see the Lua embedding socket support, cryptographic lib, json/xml support, ...
We need to wait to got a full UTF-8 or Unicode support.

# The Lua sucks ?

 * critical API are break at each new version (module definition, environment management, loading function, bitwise support, ...)
 * the easiest way to make compatibility layer to fix theAPI  need the critical API the same that is broken.
 * No reference, no official community site
 * In Lua you spend more time to find a existing module than make it your own from scratch.
 * In Lua you don't have one usual solution, you have about 10 solutions for each problem (see the choice of class system)
 * Without reference, you will have difficulty to run different solution inside the same env (like multiple implementation of class sytem)
 * ...
