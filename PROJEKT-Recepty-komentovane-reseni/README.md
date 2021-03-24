# Recepty

Bonusový úkol pro kurz Staň se kóderkou od Czechitas. Tento úkol se neodevzdává a nehodnotí. Vypracuj si ho pro sebe jako trénink kódování CSS. Toto je standardní varianta úkolu, více se dozvíš v sekci Obtížnosti úkolu.

- [Cíl úkolu](#Cíl-úkolu)
- [Grafické zadání](#Grafické-zadání)
- [Obtížnosti úkolu](#Obtížnosti-úkolu)
- [Jak si stáhnout podklady](#Jak-si-stáhnout-podklady)

Než začneš s projektem cokoliv dělat, přečti si prosím celý tento text až do konce.

Tvým úkolem je nahódovat responzivní sekci webu - můžeš si představit, že by to byla třeba vrchní část úvodní stránky webu věnovaného receptům. V této části se zobrazuje 5 vybraných receptů, které jsou právě populární. Sekce je responzivní a přizpůsobuje svůj vzhled podle šířky prohlížeče, aby na daném zařízení bylo rozložení stránky vždy co nejlepší. Na výsledný vzhled projektu se podívej na animovaném obrázku *ukazka-vysledku-responsive.gif*.

![Ukázka výsledku](ukazka-vysledku-responsive.gif)


## Cíl úkolu

Cílem projektu je procvičit si použití různých technik:
- **Responzivní webdesign**
  - stránka se musí přizpůsobovat různým šířkám prohlížeče
  - používáme princip mobile first, takže jako první nakóduj mobilní verzi, kdy jsou kartičky s recepty jen pod sebou
  - potom přidej breakpointy pro "tablet" a "pc"
  - všimni si, že vnitřek kartičky s receptem je stále stejný ve všech breakpointech - vzhled kartičky tedy stačí nakódovat v mobilní verzi a dál ho není potřeba měnit
  - jediné, co se v breakpointech mění, je minimální výška kartičky a velikosti písma, a samozřejmě také rozložení kartiček na stránce
  - nezapomeň, že když napíšeš media query doporučeným způsobem, tak vlastnosti nastavené v předchozím breakpointu se přenáší i do breakpointu dalšího. Pokud tedy např. na prvku zapneš flexbox v tabletové verzi, zůstane nastavený i pro verzi pro počítač a není ho potřeba zapínat znovu.
- **Flexbox**
  - **nepoužívej absolutní pozicování**, vše vyřeš pouze pomocí flexboxů
  - flexboxy lze do sebe vnořovat - tj. můžeš mít flexbox, který řídí rozložení kartiček na stránce, a i kartičky samotné budou malými flexboxy, které se budou starat o rozložení prvků uvnitř kartičky, a možná ještě další flexbox uvnitř jednoho z nich
  - drž se principu, že minimum kódu je vždy nejlepší cesta - i přesto, že je to příklad na flexboxy, neznamená to, že je musíš nutně použít všude a hned od začátku
  - pokud např. v mobilní verzi flexbox na něco nutně nepotřebuješ, tak ho nezapínej. Můžeš ho na daném prvku zapnout až v tabletovém breakpointu.
- **Obrázky na pozadí**
  - obrázky jídel přidej pro každý recept jako obrázek na pozadí (tj. ne jako značku `<img>` v HTML)
  - vzpomeň si na vlastnost `background-size: cover;`, která zajistí, že obrázek vždy pokryje celou kartičku, ať má jakoukoliv velikost


## Grafické zadání

Jak vypadá rozložení receptů pro mobil, tablet a počítač najdeš na obrázku *zadani-ukolu.jpg*. Najdeš tam i minimální výšky kartiček pro každý breakpoint, použité písmo a jeho velikosti.

Ve složce projektu jsou přidané obrázky s náhledem webu pro každý breakpoint:
- [náhled výsledku na mobilu](ukazka-mobil.jpg)
- [náhled výsledku na tabletu](ukazka-tablet.jpg)
- [náhled výsledku na počítači](ukazka-pc.jpg)

Kde jsou jednotlivé breakpointy najdeš i v komentáři v souboru *style.css*.

![zadání úkolu](zadani-ukolu.jpg)


## Obtížnosti úkolu

Zadání tohoto projektu je vytvořeno ve dvou úrovních obtížnosti. Tento repozitář obsahuje výchozí **standardní úroveň obtížnosti**. Pokud máš méně času nebo s úkolem hodně bojuješ, můžeš zkusit lehčí variantu úkolu.

### Standardní obtížnost
- obsažená v tomto repozitáři
- v HTML najdeš pouze obsahové elementy (nadpisy, odstavce)
- sama si do HTML musíš dopsat další strukturu, která je nutná, abys mohla HTML nastylovat podle grafického zadání
- musíš vymyslet, do jakých prvků obsah zabalíš a jaké třídy jim přidáš

### Lehčí obtížnost
- dostupná v [druhém repozitáři](https://github.com/Czechitas-Koderka-podklady/PROJEKT-Recepty-lehci)
- grafické zadání je stejné, ale v HTML je kompletně připravený obsah včetně struktury, obalových prvků a přidaných CSS tříd
- v této obtížnosti nemusíš HTML vůbec upravovat - stačí si ho prostudovat, abys věděla jaké prvky/třídy máš stylovat a "jenom" k nim napsat CSS

Je úplně v pořádku, pokud si nakonec zvolíš jednodušší variantu (např. kvůli nedostatku času), ale doporučuji, abys nejprve zkusila standardní obtížnost, kde si musíš sama vytvořit i HTML strukturu a pojmenovat CSS třídy. Není to zase o tolik těžší a v reálném životě ti také nikdo HTML připravovat nebude. Jako kóderka dostaneš grafický návrh a ten budeš muset převést do HTML a CSS. Budeš-li si u bonusových úkolů volit jednodušší obtížnosti, nakonec zjistíš, že sice umíš CSS, ale dělá ti problém vymyslet a napsat si vlastní HTML.


## Jak si stáhnout podklady

1. Udělej si **fork** této repozitáře - tím se ti úkol zkopíruje do tvého GitHub profilu.
2. Forknutou repozitář si naklonuj k sobě na disk.

Pokud nevíš, co je to **fork repozitáře** a jak ho provést, podívej se na [krátké video](https://youtu.be/K7rE3jRCjD4).

