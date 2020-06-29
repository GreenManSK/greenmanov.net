---
layout: post
title: "Konachan.com downloader"
date: 2012-02-25 09:00:00 +0200
permalink: /2012/konachan-com-downloader/
category: "Programy"
tags: anime, C#, ľudská hlúposť, php, programovanie, šialenstvo, závislosť
image: /assets/img/2012/f9f80de90b7b39cf18bf6f0ef41b0701-300x225.jpg
imagelink: /assets/img/2012/f9f80de90b7b39cf18bf6f0ef41b0701.jpg
---
Keďže o sebe s obľubou tvrdím, že som grafik a programátor je dosť divné, že väčšina článkov na tomto blogu sa točí okolo anime. Hlavným dôvodom je, že to flákam a tak som sa rozhodol pochváliť sa tu aj tými menšími blbostičkami, čo z času na čas splodím. Ako čiastočný potomok ľudského rodu som samozrejme lenivý a ako „programátor“ ešte viac. A preto si rád uľahčujem život niekoľko riadkovými kódmi, ktoré sú schopné ma väčšinou z 90% nahradiť (tých 10% je len užívanie si výsledku práce). A tu môžem začať rozprávať tento nový príbeh o tom, ako som po dlhej dobe programoval užitočnú vec.

Tých pár ľudí, čo ma sleduje na [Twitteri](https://twitter.com/GreenManSK) alebo na všetkými nenávidenom Facebooku (Z bezpečnostných dôvodov odkaz chýba. Bojím sa šialených fanúšikov.), si mohli všimnúť, že som nedávno dopozeral anime [Mahou Shoujo Madoka Magika](http://anidb.net/perl-bin/animedb.pl?show=anime&aid=8069) (Áno, už zasa anime…) a veľmi sa mi páčilo. Po grafickej stránke bolo veľmi pekné a vďačné, takže mi bolo hneď jasné, že sa nájdu stovky krásnych pozadí s týmto anime. A tak som zablúdil na [konachan.com](http://konachan.com/) (v tejto dobe moja obľúbená stránka s pozadiami) a zadal si do vyhľadávania „mahou_shoujo_madoka_magica“ a kde sa vzalo, tu sa vzalo vybehol na mňa počet strán 83 strán obrázkov. A mne bolo jasné, že ich budem chcieť väčšinu. [Filozofická vsuvka: Nie som si istý, či som úchylný lebo ich chcem všetky alebo ich chcem všetky pretože som úchylný.] Po 7 stranách mi došlo, že by som tu bol ešte 6,4 rokov pokiaľ by som to prešiel všetko a tak sa vo mne zobudil niečo, čo spalo v najtemnejšej časti môjho sveta… Áno, presne to. Môj vnútorný programátor. Keďže som primárne PHPčka a venujem sa mu už nejaký ten piatok (Niekto mal kamarátov ja som sa hral do noci s PHP.), začal som bez premýšľania robiť v ňom. Lenže PHP nie je práve najmenej náročné, hlavne keď ide o veci na ktoré nebolo navrhnuté. Aj keď som mal program za menej ako hodinu, to ako sa choval k môjmu PC sa mi už tak veľmi nepáčilo. A mať zapnutý jeden prehliadač navyše aby som mal istotu, že sa všetko stiahlo bolo dosť nepraktické.

A tak som sa chopil mojich mizerných znalostí C# a výborných znalostí Googlu a začal prerábať program do C# a jeho .NET Framework (Keby som pri PHP neprestal s [nette](http://nette.org/) bolo by to len zjednodušenie :-D). Zabralo to síce o 3 hodiny viac ako pôvodný PHP kód, má to 5krát viac riadkov a nevyznám sa v tom tak dobre, ale funguje a rád by som sa o neho podelil s vami. Viem, že sa nájde niečo jednoduchšie a lepšie, ale tu šlo nácvik a lenivosť hľadať to. A predsa len vypadá to husto keď vám ploche beží niečo takéto.

[![Konachan Downloader](/assets/img/2012/konachan-300x153.jpg)](/assets/img/2012/konachan.jpg)

Do budúcna plánujem možnosť sťahovania viac tagov naraz, aby ste si mohli dať napríklad na noc stiahnuť miliardy pozadí z obľúbených anime alebo priaznivejšie UI. Vychádzal som len zo znalostí čo mám a tie sa točia len okolo konzole.

A ako táto zrúdička vlastne funguje? Najprv zadáte tag ktorý chcete stiahnuť. Ide vlastne o presný text z vyhľadávacieho poľa. Napr. „suzumiya_haruhi“ pre všetky obrázky s Haruhi, „k-on! rating:questionable“ pre všetky obrázky z K-On! z kategórie Ecchi alebo „rating:explicit“ pre váš milovaný obsah +18. Jediný problém je, že to musíte prepísať ručne. To vás donúti si rozmyslieť, či si stiahnete všetko alebo len tie vaše prasačinky.  Ďalej zadáte stránku od ktorej chcete začať sťahovanie a nakoniec stránku po ktorú chcete sťahovať. Pár slovíčok, 2 čísla a môžete čakať a na krásnu odmenu.

[Sťahovať môžete tu!](/assets/Konachan-downloader-v2.rar)

Keďže ide o program v C# musíte mať [.NET Framework](http://msdn.microsoft.com/en-us/netframework/aa569263), takže Mappláci majú smolu. Dúfam, že vám program pôjde a bude sa vám hodiť, ak nie tak nahláste a pokúsim sa to opraviť/pomôcť vám. Zatiaľ Green! Mňa ešte čaká roztriediť 640 obrázkov na tie ktoré chcem, nechcem a sliepky s kravatou.
