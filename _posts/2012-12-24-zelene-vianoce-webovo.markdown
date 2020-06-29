---
layout: post
title: "Zelené Vianoce webovo"
date: 2012-12-24 09:00:00 +0200
permalink: /2012/zelene-vianoce-webovo/
category: "Tvorba webov"
tags: css, experiment, javascript, Lightning Soft, tvorba webov, webdesign
image: /assets/img/2012/christmas-e1356355347503-300x300.jpg
imagelink: /assets/img/2012/christmas.jpg
---
Už som sem zasa nejaký ten mesiac nič nenapísal, a tak som sa rozhodol to napraviť. A keď už máme dnes ten Štedrý deň, bude to trochu vo vianočnej nálade. Ale aby som sa držal zvyku tak vám najprv niečo zaželám.

*Prajem vám zelené Vianoce a zelený nový rok. Nech sa vám splnia všetky vaše priania, nech máte lolitiek po… koľko chcete. Nech vám vaša 2D waifu splní všetko, čo chcete a nájdete plno dobrých doujinshi s ňou v hlavnej roli. A hlavne, nech mám zo všetkého toho profit aj ja!*

A tento rok som prichystal so [Satikom](https://satik64.com/) aj prianie od [Lightning Softu](https://www.lightningsoft.org/cs/). [Prianie môžete nájsť tu](http://vanoce.lightningsoft.org/) a o ňom bude dnešný článok.

Hlavú časť grafiky na tomto krásnom prianiu urobil Satik64, moja je len grafika tímu, zelenej postavy z [Warped Times]({% post_url 2011-06-24-warped-times-2 %}) a pár lóg k hrám. Hlavná náplň mojej práce bola kódenie. Nie je to nič špeciálne, ale chcel by som sa pochváliť, čo som použil. A hlavne, ako také malé veci pomáhajú v učení sa nových technológií.

Každý má rád nové veci, že? Teda každý nie, ja sa ich bojím a to hlavne vo webových technológiách, kde vďaka rozmanitému výberu prehliadačov, neviete presne, čo kde ako pôjde hneď. Hlavne kvôli demen… používanému Internet Exploreru, ktorý je bežný hneď v niekoľko verziách. Aj keď na starú šiestu verziu som sa už vykašlal, furt je to niekedy dosť práce. Hlavne s CSS3 a HTML5, o ktorom sa pri nich dá len snívať.

S Css3 sa zahrávam už dlhšiu dobu, ale stále som mal problém s tým, čo kde ako fungovalo. Že niekde ten tieň nebude a rohy budú niekde ostré a niekde zaoblené. Pri riešení takýchto problémov som sa nedávno dostal ku knižnici, ktorú som si aj pri tejto malej zábavke mohol vyskúšať a ešte viac pochopiť, ako veľmi užitočná je. Ide o Modernizr, je to knižnica v JS, ktorá pomáha zistiť, či je daná vlastnosť z CSS3 alebo kód z HTML5 funkčný v prehliadači. A ak nie je, dovolí urobiť potrebný kód. Ak si hovoríte, ako ja dlhé roky, že JS nemusí mať každý, takže to nerieši problém úplne poviem vám to tak. Ľudí bez JS sa tak veľa nenájde a ak už nejaký inteligent chodí po internete bez neho a stále čaká, že všetko bude vypadať úžasne, tak by sa mal dať liečiť. V tomto projekte mi vyriešila 2 problémy.

Prvý bolo zjemnenie okrajov obrázku do čierna, keďže pôvodný bol nezaobalený. Jasne, mohol som ho rovno prerobiť tak, aby už v ňom bol čierny okraj, ale prečo? Čo ak by si ho niekto stiahnuť a dať na pozadie? (Blbší dôvod ma aktuálne nenapadá.) Tak som to vyriešil s CSS3 a jeho box-shadow. Lenže tu nastal problém, keď prehliadať box-shadow nepodporoval a obrázok tam bol zasa škaredo zasadený do pozadia. Tu mi pomohol [Modernizr](http://modernizr.com/), ktorý keď zistí, že prehliadač nepodporuje box-shadow, ho nahradí za priesvitný obrázok s tieňom. A prečo som to celé cez tento obrázok? Pri takto malom projekte je to nič, ale predstavte si veľký projekt. Navštívia ho denne miliardy ľudí a prenos dát je obrovský, takto som ušetril terabajty dát tým, že nie každému sa stiahne.

Ďalej som použil HTML5 a jeho audio, aby v pozadí mohla hrať vianočná pesnička. Tu nastal problém s ovládaním zvuku, ktoré sa zobrazovalo aj v prehliadačoch, kde hudba proste nehrala. Ale tu znova letí na pomoc Superma… Modernizr s jeho detekciou podpori tagu &lt;audio&gt; a v prípade, že ju nezistí ovládanie hudby schová. Ďakujem Modernizr, zachránil si milióny životov ľudí, čo by tam to ovládanie mali a zabili by sa, lebo by im nefungovalo.

A nakoniec už len taká malá blbostíčka, ale predsa. Aj keď Javascript používam dnes už celkom často, tak v ňom proste nie som tak zbehnutý, ako napr. v PHP, takže malý nácvik sa vždy hodí.

Takže už som vám zaželal, ďakujem, že ste v tento sviatočný deň zabili pár minút život a u mňa a tak. Po novom roku mám v pláne 2 články. Sociálne experimenty stoja, ale pohrávam sa v hlave s určitým nápadom ktorý by ich mohol pár priniesť. Green!

A ešte nejaká tá pesnička aby sa vám lepšie čakalo na večeru.

{% include youtubePlayer.html id="b2d7UhK5SAE" %}
