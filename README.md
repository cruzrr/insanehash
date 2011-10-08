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
  * The 32-bit Keccak version Keccak[256, 544, 0] is supported in keccak32.js and keccak32.min.js as my "shortest available implementation" version.
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
3. Put `var insane = require('./insanehash').crypto;` in your app.js (or where you want). PS: **.crypto** = namespace ;)  
4. Call `insane.skein('Hi!');` where you want. PS: **.skein** is one of the six implemented algorithm. 
5. You will get this **string**: **6dbe952ab5ec3bf45a82887953953e3220e1eab7ae9069ae548ac8561691378993210ca0cb0666656614ef858fca9893a9bb6fe149dca792c910d6518aecdd30**  

The workaround way -> **sorry ;(**  

1. Download it.  
2. Put the file **in a insanehash directory** (_create one_) at the **node_modules folder**.  
3. Put `var insane = require('insanehash').crypto;` in your app.js (or where you want). PS: **.crypto** = namespace ;)  
4. Call `insane.skein('Hi!');` where you want. PS: **.skein** is one of the six implemented algorithm.  
5. You will get this **string**: **6dbe952ab5ec3bf45a82887953953e3220e1eab7ae9069ae548ac8561691378993210ca0cb0666656614ef858fca9893a9bb6fe149dca792c910d6518aecdd30**  

#Sua procura acabou!

* Você precisa de criptografia de **verdade** e **séria**?  
* Você acha que o MD6 já é velho (e fraco) e quer algo como os **algoritmos finalistas para o SHA3**?  
* Você usa o **NodeJS**, sabe que existe boas bibliotecas por ai, mas você é do tipo **cutting edge**?  

Então relaxa, pois **realizei seu sonho**! :)  
Conheça o **InsaneHash** (_logo no NPM install -g mais perto de você_).

OBS: Em **Javascript**, claro!