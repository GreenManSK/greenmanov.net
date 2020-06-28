---
layout: post
title:  "Optimalizácia pre prehliadače"
date:   2011-03-23 08:08:00 +0200
permalink: /2011/optimalizacia-pre-prehliadace/
category: "Tvorba webov"
tags: css, optimalizácia, tvorba webov
---
Zasa prebehol nejaký čas od môjho posledného článku na blogu, a tak som sa rozhodol napísať nový. Najprv by som rád vyhodil ľudí čo sem klikli pretože čítali názov článku ako „Optimalizácia pre vyhľadávače“(pre priaznivcov Petra Hejla hledače). Tento článok je o optimalizácii stránok pre prehliadače, keďže ako každý z vás vie, alebo čoskoro bude vedieť, každý prehliadač zobrazuje stránky rôzne.

O tom ako tento problém vznikol bolo už napísané veľa krát a bolo by to skôr na článok o histórii stránok. Stačí vám vedieť že hlavný podiel na bezosných nociach tvorcov webov má Microsoft a jeho Internet Explorer ktorý ako naschvál nikdy nepracuje tak ako by ste chceli, alebo to od neho čakali. Ale aby som M$ len nekrivdil poviem vám strašnú pravdu. Aj v iných prehliadačoch môžu nastať rozpory a niekedy dokonca horšie ako v IE, IE vám web proste celý zničí ale prehliadače vyššej úrovne(Google Chrome, Opera…) vám stránku môžu zničiť na malých detailoch ktoré sú v ich jadrách rozdielne.

Určite si hovoríte „GreenMan čo to trepeš? V mojom prehliadači to ide dobre a iný používajú len lami!“. Je to pravda, ale lám čo používajú napríklad IE bolo vo februári ešte 26,5%.Na presné štatistiky sa môžete pozrieť v [škole](http://www.w3schools.com/browsers/browsers_stats.asp). Podiel IE6 našťastie klesá pretože on býval najväčší problém, ale priznajme si to. Ja a pravdepodobne aj vy robíte stránky pre český/slovenský trh, a tam warez Windows XP prekvitá. A na každom správnom XP čo okolo legálnej verzii ani nechodilo je IE6.

Tak teoretickú časť by sme mali hotovú. Môžeme prejsť na tú praktickú. Najprv by som vám rád dal do rúk nástroj za ktorý ma budete uctievať ak o ňom neviete. Volá sa Browsers Shots a nájdete ho na adrese [www.browsershots.org](http://www.browsershots.org/). Na tejto stránke len vložíte URL adresu vašej stránky, vyberiete si v ktorom prehliadači a pod aký OS ju chcete zobraziť, možno upravíte nastavenia zobrazenia a stlačíte na Submit. A o pár minút máte hotový celý fotoalbum vašej stránky v rôznych prehliadačoch. Ak plánujete fotiť veľa a často doporučujem vám registrovať sa pretože aspoň mňa to ako neregistrovaného obmedzilo na určitý počet snímok. Problém ale je že vám to dá len fotku a stránku už musíte mať niekde zobrazenú na ostro a nie doma na localhoste.

Fotenie môže byť zdĺhavé a musím vám povedať že CSS nie je jediná vec ktorú každý prehliadač spracováva inak. Aj Java Script sa nevyhol tomuto problému preto potrebujete niečo viac pojazdné. Preto by bolo najlepšie mať v PC aspoň základné prehliadače na test. Ja osobne mám v PC [Google Chrome](http://www.google.com/chrome), [Operu](http://www.opera.com/), [Firefox](http://www.mozilla.com/sk/firefox/) a Afri… myslel som [Safari](http://www.apple.com/safari/). Pri týchto prehliadačoch je bežné že používatelia majú najnovšiu verziu alebo tam rozdiel v týchto veciach nie je až taký priepastný ako pri osudovom IE.

Poviete si „Fajn mám aj nejaké IE v PC mám pokoj.“  To je veľká chyba! Pretože pri IE nikdy neviete čo urobí a rozdiely sú až príliš veľké. Preto potrebujete mať v PC IE6, 7, 8 a nové 9. Lenže tu je problém že M$ vám dovolí mať v PC len jeden a k tomu nemôžete ísť na nižšiu verziu. Preto boh povedal „Budiš IETester!“ Nie je to program v ktorom si vyskúšate ktorý IE chcete používať ale otestujete tam svoje stránky. Nájdete ho na  tejto [stránke](https://www.my-debugbar.com/wiki/IETester/HomePage). Tento program má v sebe to najväčšie zlo sveta od verzii 5.5 po 9 takže vám pomôže aj keď je to furt dosť zložité.

Dúfam že sa vám článok páčil a pomohol vám. Namakal som sa na tom takže chcem kritiku(napíšte zlé slovo a ste mŕtvy). Mohol by som napísať aj kódovú časť ak by bol záujem ale to pochybujem. Ak máte záujem napíšte do komentárov(E-Mail zadajte kludne aj jozko.mrkvicka@domena.xxx chcete ak je v tom problém).
