---
layout: post
title:  "Cool URL bez mod_rewrite"
date:   2011-06-05 08:08:00 +0200
permalink: /2011/cool-url-bez-mod_rewrite/
category: "Tvorba webov "
tags: cool url, mod_rewrite, php, tvorba webov
---
S problémom hostingu, kde nie je mod_rewrite povolený, som sa stretol už dávno. A jeden z nich je aj IC.cz, na ktorom hostujem ja. Pred mesiacom som si kúpil knihu [1001 Tipů a triků pro PHP](http://knihy.cpress.cz/1001-tipu-a-triku-pro-php.html) od [Jakuba Vrány](http://www.vrana.cz/) a tam som sa dočítal o teoretickom postupe ako mať na stránke Cool URL aj bez mod_rewrite. A tak som sa rozhodol si pre to napísať knižnicu v PHP a poskytnúť ju svetu.

Pre tých čo nevedia čo to Cool URL sú, je tu malé zhrnutie, ak to viete môžete tento odsek preskočiť. Cool URL je URL oveľa vizuálne krajšia a pre používateľa ľahšie zapamätateľná. Porovnajte si napríklad „www.priklad.sk/?clanok=12“ a „www.priklad.sk/novy-clanok/“.  Tento typ URL je vraj výhodný aj pre vyhľadávač pretože dané kľúčové slovo vidí aj v URL adrese.

Základné technické požiadavky na knižnicu sú PHP5 alebo vyššie a mať zapnutú v Apache konfiguračnú direktívu AcceptPathInfo. Väčšina dnešných hostingov toto spĺňa. Zapojiť knižnicu do už fungujúcej stránky nie je problém keďže je schopná automaticky presmerovať z URL starého typu na nové(do môjho starého a neprehľadného RS som ju zapájal asi hodinu, a to som sa mu v zdrojovom kóde nevŕtal rok 😀).

Stiahnuť ju môžete tu:
[CoolUrl_1.0](/assets/CoolUrl_1.0.zip)

Zip obsahuje dva súbory, jeden je prehľadný kód knižnice a druhý je jej zredukovaná verzia. Vloženie do stránky je veľmi jednoduché. Knižnica sa musí načítať a spustiť pred akýmkoľvek vypísaním textu keďže používa funkciu <code>Header()</code>.

<pre>&lt;?php
    require_once 'CoolUrl.php';
    $coolUrl = new CoolUrl($model, $separator, $array);</pre>

Prvá premenná <code>$model</code> je určená pre model URL adresy stránky. Jednotlivé premenné sa zapisujú medzi <code>@@</code>, napríklad <code>@premenna@</code>. Pre názvy premenných platia rovnaké pravidlá ako pre premenné v PHP. Jednotlivé premenné sa oddeľujú znakom <code>/</code>. Model môže vypadať napríklad takto: <code>clanok/@nazov@</code>, <code>@nazov@/@id@</code>.

$separator sa automaticky dáva na koniec modelu a nahrádza znaky <code>/</code> v modeli. Automaticky je nastavený na <code>/</code>, takže pri vytváraní ho nie je povinné zadať.

$array je pole do ktorého sa uložia premenné z URL, automaticky je nastavená na <code>$_GET</code>, takže nie je povinné ho zadať.

Nevýhoda týchto URL je, že fungujú na základe ukladanie časti URL po .php do premennej <code>$_SERVER[‚PATH_INFO‘]</code>. Tým pádom vypadajú takto: <code>clanok.php/nazov-clanku/</code>. Toto chovanie sa dá ale obísť ak sú na Apache servery zapnuté vloby Options MultiViews a MultiviewMatch Handlers. Tento spôsob používa napríklad [Wikipedia](http://www.wikipedia.org/).

Knižnicu môžete voľne používať ako chcete stačí uviesť autora. Ak sa chcete takýchto zaujímavostí dozvedieť viac, odporúčam vám kúpiť si knihu [1001 Tipů a triků pro PHP](http://knihy.cpress.cz/1001-tipu-a-triku-pro-php.html).

V poslednej dobe som dostal nápad ešte na najmenej jeden článok, takže čoskoro tu možno bude ďalší článok.
