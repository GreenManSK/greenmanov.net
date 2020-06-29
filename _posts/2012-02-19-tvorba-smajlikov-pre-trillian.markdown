---
layout: post
title: "Ako maličkosti menia život"
date: 2012-02-19 09:00:00 +0200
permalink: /2012/tvorba-smajlikov-pre-trillian/
category: "Programy"
tags: epické, facepalm, ľudská hlúposť, Trillian
image: /assets/img/2011/Final_Icon_-_Test_8_-_256_reasonably_small.png
imagelink: /assets/img/2011/Final_Icon_-_Test_8_-_256_reasonably_small.png
---
O tom, čo je [Trillian]({% post_url 2011-11-08-trillian-najlepsi-klient-na-chatovanie %}) som tu už písal. Tento návod nemá veľmi veľký význam pre ľudí čo ho nepoužívajú a tak to nemusím vysvetľovať znova. V skratke je to IM klient, ktorý krásne zvláda ICQ, Skype, Facebook, Twitter a plno ďalších prostriedkov na chatovanie a zdieľanie informácií. Celý je dosť prispôsobivý a tak nie je problém si zmeniť vzhľad, smajlíky alebo zvuky. Lenže nie každému stačí to, čo si nájde na internete na stiahnutie. A tak isto som na tom ja. Keďže mám veľmi dobrú mienku o ľudstve a často si ju znova a znova dokazujem, je mojím bežným zvykom používať takzvaný [facepalm](/assets/img/2012/24dc476c926190_full.jpg). Niekedy mi stačilo používať prosté „omg“ alebo „to je idiot…“, ale po tom ako som sa naučil používať vo Facebook chate vkladať profilové fotky a začal tam používať tento [facepalm](https://www.facebook.com/Kyon-Facepalm-190557937684900/), začalo mi to chýbať všade. A tak som sa rozhodol, že si takéhoto „smajlíka“ pridám aj do svojho milovaného Trillianu a naučím to aj vás. A pritom vás naučím prirodzene používať tento boží dar, zvaný facepalm.

Ako prvé budeme potrebovať nainštalovaný [Trillian](http://www.trillian.im/), ale to už určite došlo každému. Ak nie tak potom použijeme facepalm. Ďalej si nájdeme súbor do ktorého sme si ho nainštalovali. U mňa je to napríklad „C:\Program Files (x86)\Trillian“, pri ne64bitových verziách Windowsu to bude bez (x86) a aj označenie [HDD]http://sk.wikipedia.org/wiki/Pevn%C3%BD_disk sa môže líšiť. Tam si otvoríme priečinok „stixe“ a v ňom priešinok „plugins“. Gratulujem, práve ste sa dostali na miesto kam sa vkladajú vaše pluginy. Ak ste sa tam nedostali použijeme facepalm. Základné smajlíky sú v priečinku „TP21Emoticons-16×16“. Nové si môžete stiahnuť [tu](http://developer.ceruleanstudios.com/index.php/EmoticonPacks) alebo pohľadať napríklad na mojom milovanom [DeviantARTe](http://www.deviantart.com/). Ja používam sadu „Riceballs 2010“. Keď máme vybratú sadu smajlíkov, ktorú chceme upraviť otvoríme si jej priečinok. Uvidíme pár obrázkov smajlíkov a niekoľko ďalších súborov. Pre nás je najdôležitejší „main.xml“. Ale najprv si nájdeme obrázok pre nového smajlíka, po pár sekundách [googlenia](http://lmgtfy.com/?q=kyon+facepalm) (Ak ste na to klikli použijeme facepalm.) som našiel [túto nádheru](/assets/img/2012/facepalm.gif). Tú vložíme do priečinka k smajlíkom.

Otvoríme si súbor „main.xml“, ktorý je napísaný v XML. Pre tých, čo nevedia (Správne! Zasa facepalm.), XML je značkovací jazyk rovnako ako napr. HTML až na to, že sa dá jednoduchšie využívať ako databáza a podobné veci a preto sa využíva pri dosť veľa programoch, ale aj napríklad také RSS je v XML. Prvé čo urobíme je, že si nájdeme posledný tag s názvom „bitmap“, u mňa vypadal takto:

<pre>&lt;bitmap name="thumbsdown" file="../../stixe/plugins/Riceballs2010/thumbsdown.png"/&gt;</pre>

Argument name udáva názov vašeho nového smajlíka, v našom prípade ho nazveme „facepalm“. file je zasa odkaz na súbor, pri ňom meníme len koniec s názvom obrázku, „facepalm.gif“. Na nový riadok za posledný tag „bitmap“ teda vložíme niečo takéto:

<pre>&lt;bitmap name="facepalm" file="../../stixe/plugins/Riceballs2010/facepalm.gif"/&gt;</pre>

Ak ste už odišli s tým, že máte hotovo použijeme facepalm. Ešte musíme zadať, za aký text sa bude náš [facepalm](/assets/img/2012/facepalm.gif) vymieňať. Nájdeme si posledný tag „emoticon“. Vypadá nejak takto:

<pre>&lt;emoticon text= "u_u" &nbsp; &nbsp;&gt;&lt;source name= "sarc" &nbsp;left=" 0" right=" 18" top=" 0" bottom=" 18"/&gt;&lt;/emoticon&gt;</pre>

„text“ udáva za aký text sa bude vymieňať, takže zadáme „(facepalm)“. „name“ zadáme také isté ako pri tagu „bitmap“. A nakoniec, argumenty „left“, „right“, „top“ a „bottom“ udávajú súradnice na obrázku, podľa ktorých sa bude zobrazovať. Ak je to na vás príliš zložité, facepalm, zadajte do „left“ a „top“ 0 a do „right“ a „bottom“ šírku a výšku obrázku. Ak chcete aby sa váš smajlík nahrádzal za viac textov, „(facepalm), (kyon), (kyonfacepalm)“ tak vytvoríme viac nových tagov „emoticon“ s iným textom. Výsledok bude vypadať nejak takto:

A výsledok?

[![Trillian](/assets/img/2012/AlordfzCMAAb7iO-225x300.png)](/assets/img/2012/AlordfzCMAAb7iO.png)

Teraz by ste už mali byť schopný vytvoriť si novú vlastnú sadu smajlíkov upravovaním pôvodnej. Na koniec vám dám na stiahnutie upravenú verziu Riceballs 2010 s [Kyonovim facepalmom](/assets/img/2012/facepalm.gif). [Sťahujte tu](/assets/Riceballs2010.rar). Ak budete mať nejaký problém stačí napísať do komentárov alebo na nejaký kontakt na podstránke O mne, rád pomôžem. Tak už vám len prajem veľa šťastia a じゃあね。\[džá ne] Tento týždeň som sa konečne naučil hiraganu tak musím machrovať. (Ospravedlňujem sa zástancom iného prepisu, ale nikdy neviete, či to nebude čítať niekto kto neprečíta „jaa ne“ poriadne. Veď viete facepalm.)
