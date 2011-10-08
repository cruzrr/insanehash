#Your search over!

* Do you need a **fast** and **seriously** cryptography?
* Do you think that **MD6 is too old** (*and poor*) and want something like the **finalists of the CHAC** (**C**ryptographic **H**ash **A**lgorithm **C**ompetition) of NIST for **SHA3**?
* Do you use the **NodeJS**, knows that there is good libraries out there, but what you **really want** is something **cutting edge**?

So **relax**, because your dream **was realized**! :)  
Meet **InsaneHash** (soon in the "*npm install -g*" closer to you).

## OK! What's **insanehash?**  
The **lastest SHA3 cryptographic hash algorithm from NIST Hash Competition** based on [**Chris Drost implementation**](https://github.com/drostie/sha3-js) writed in **Javascript** and for **NodeJS**

## About algorithms:  

* **BLAKE**, by Aumasson, Henzen, Meier, and Phan  
  * BLAKE-32 is supported in blake32.js and blake32.min.js
* **BMW (Blue Midnight Wish)**, by Gligoroski, Klima, Knapskog, El-Hadedy, Amundsen, and Mjølsnes
  * BMW256 is supported in bmw.js and bmw.min.js
* **CubeHash**, by Dan Bernstein.
  * CubeHash16/64-256 is supported in cubehash.js and cubehash.min.js
* **Keccak**, by Bertoni, Daemen, Peeters, and van Assche
  * The 64-bit SHA3-256 candidate Keccak[1088, 512, 32] is supported in keccak.js and keccak.min.js as a "standards-compliant" version.
* **Shabal**, by Bresson, Canteaut, Chevalier-Mames, Clavier, Fuhr, Gouget, Icart, Misarsky, Plasencia, Paillier, Pornin, Reinhard, Thuillet, and Videau
  * Shabal-256 is supported in shabal.js and shabal.min.js.
* **Skein**, by Bellare, Callas, Ferguson, Kohno, Lucks, Schneier, Walker, and Whiting
  * Skein-512-512 is supported in skein.js and skein.min.js for standards-compliance.
  * A 32-bit Skein-256-256 (non-compliant) version is supported in halfskein.js and halfskein.min.js as a shorter algorithm.

##How to use **insanehash**?
Ridiculously, creepily very simple!  

The easiest way:  

1. Download it.  
2. Put the file **at the root of you application**.  
3. Require it as `var insane = require('./insanehash').insanehash;` PS: `.insanehash` = namespace ;)  
4. Call this. You will get a **string** with the hash.
  * `insanehash.blake32('Hi!');` -> 'ceb42cb8ab21fe511b85ecd74933b9f4aafa4d1c67da0778b69e375245942314'  
  * `insanehash.shabal('Hi!');` -> '0427065214b9a8ea2d79c73a1a2d02ea3f9c4f71d4c73a30ad2c0bc8b1c172d9'  
  * `insanehash.bmw('Hi!');` -> '44fe7f399277b09b8e892a80522b833703abacd5fc7f71da6db96999ca4bdb06'  
  * `insanehash.skein('Hi!');` -> '6dbe952ab5ec3bf45a82887953953e3220e1eab7ae9069ae548ac8561691378993210ca0cb0666656614ef858fca9893a9bb6fe149dca792c910d6518aecdd30'  
  * `insanehash.cubehash('Hi!');` -> 'a206bffa3c77a6410270f061e6b264fd79d1a997c06d444ee1bba42cff2b66d3'  
  * `insanehash.halfskein('Hi!');` -> '39edf053bf6be95f1af2476f83fbf9b71fa0e3188361def18c879a9f09370f8a'  
  * `insanehash.keccak('Hi!');` -> '22dd5d47d9cb35a05e3022a7bac1a39547da7b303aba89cbe9205046d1f0762c'  

The workaround way: (**it will be different soon, i promisse!**)  

1. Download it.  
2. Put the file **in a insanehash directory** (_create one_) at the **node_modules folder**.  
3. Put `var insane = require('insanehash').insanehash;`