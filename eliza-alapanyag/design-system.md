# Eliza Beauty Salon – design system

## Hangulat

Nőies, elegáns, nyugodt, prémium, de barátságos. Olyan, mint egy csendes, világos szalon természetes anyagokkal: sok levegő, meleg krém- és bézstónusok, mély zsályazöld kiemelések és finom barna részletek.

**Ne legyen:** csillogó, rózsaszín-giccses, túldíszített, harsány. Ne legyen benne neon, erős színátmenet, sötét mód vagy „tech startup” hatás.

## Színek

| Szerep | Név | Hex | Mire |
|---|---|---|---|
| Elsődleges | Mély zsályazöld | `#6F7666` | Gombok, ikonok, hangsúlyos vizuális elemek |
| Elsődleges sötét | Sötét zsályazöld | `#50594A` | Gomb hover, aktív állapot, linkek és kisebb zöld szövegek világos háttéren |
| Másodlagos zöld | Világos zsálya | `#ACB09A` | Dekoratív felületek, kiemelt kártyák, kisebb háttérblokkok |
| Akcentus | Meleg barna | `#B8936D` | Csak díszítés: vékony vonalak, kis ikonok, számok sötét háttéren.  **Világos háttéren szövegre nem jó.** |
| Háttér | Meleg krém | `#F8EFE9` | Az oldal alap háttere |
| Felület | Púder | `#F1E6DF` | Váltakozó szakasz-háttér, kártyák |
| Szöveg | Sötét kakaó | `#2E2626` | Törzsszöveg, címsorok |
| Másodlagos szöveg | Szürkésbarna | `#6B5F5C` | Leírások, kisebb szövegek, űrlap-címkék |
| Vonal | Halvány púder | `#E3D6CF` | Elválasztók, űrlapmezők kerete |
| Sötét szakasz | Sötét kakaó | `#2E2626` | Lábléc, egy-egy kiemelt CTA-sáv, krém (`#F8EFE9`) szöveggel |

Ellenőrzött kontrasztok (WCAG AA, normál szövegre min. 4,5:1): sötét kakaó krémen 13,0; másodlagos szöveg krémen 5,4, púderen 5,0; fehér mély zsályazöldön 4,7; sötét zsályazöld krémen 6,5; sötét kakaó világos zsályazöldön 6,6; meleg barna sötét kakaón 5,2.

Fontos: mély zsályazöld gombon fehér szöveget használjunk, ne krémszínűt. Világos háttéren a kisebb zöld szövegekhez a sötét zsályazöld (#50594A) használható. A világos zsályazöld (#ACB09A) dekoratív felületszín, rajta sötét kakaó szöveggel. A meleg barna (#B8936D) világos háttéren csak dekorációra használható.

## Betűtípusok

Mindhárom ingyenes, a Google Fontsról tölthető be, és van benne magyar ékezet (ő, ű).

- **Címsor:** DM Serif Display, 400 vastagság. Elegáns, karakteres talpas betű.
- **Törzsszöveg:** DM Sans, 400 és 500 vastagság. 
- **Dekoratív felirat:** Licorice, 400 vastagság. Finom, kézírásos betű, kizárólag rövid díszítő szövegekhez, például a hero szekcióban vagy egy mottónál.
- **Gombok, kis feliratok (kicker):** DM Sans 500, nagybetűvel, 0,08em ritkítással.

### Méretskála (desktop / mobil)

| Elem | Betű | Desktop | Mobil | Sormagasság |
|---|---|---|---|---|
| H1 | DM Serif Display 400 | 60px | 38px | 1,1 |
| H2 | DM Serif Display 400 | 44px | 32px | 1,15 |
| H3 | DM Serif Display 400 | 28px | 24px | 1,2 |
| Kicker | DM Sans 500, nagybetű | 14px | 13px | 1,4 |
| Törzs | DM Sans 400 | 18px | 16px | 1,65 |
| Kis szöveg | DM Sans 400 | 15px | 14px | 1,5 |
| Gomb | DM Sans 500, nagybetű | 15px | 15px | 1 |
| Dekoratív felirat | Licorice 400 | 40px | 30px | 1,2 |

## Térközök és elrendezés

- Alapegység **8px**: minden térköz ennek többszöröse (8, 16, 24, 32, 48, 64, 96, 128).
- Szakaszok függőleges térköze: desktopon 96–128px, mobilon 64px.
- Tartalom maximális szélessége: 1200px; folyó szöveg max. 680px széles.
- Oldalsó margó mobilon: 20px.

## Komponensek

- **Elsődleges gomb:** mély zsályazöld (#6F7666) háttér, fehér szöveg, 16px × 32px belső térköz. Aszimmetrikus, levélformájú lekerekítés (border-radius: 0 32px 0 32px): a jobb felső és bal alsó sarok lekerekített, a másik kettő szögletes. Hoverre sötét zsályazöld (#50594A). A felirat legyen középre igazítva, megfelelő távolságra a lekerekített szélektől.
- **Másodlagos gomb:** átlátszó háttér, 1px sötét zsályazöld (#50594A) keret, sötét zsályazöld szöveg, ugyanaz az aszimmetrikus, levélformájú lekerekítés (border-radius: 0 32px 0 32px). A felirat itt is középre igazított, megfelelő belső térközzel.
- **Kártya:** púder, fehér vagy világos zsályazöld (#ACB09A) háttér, finoman levélformát idéző aszimmetrikus lekerekítés (border-radius: 12px 48px 12px 48px). A jobb felső és bal alsó sarok erősebben, a másik kettő enyhén lekerekített. Nincs vagy csak nagyon halvány árnyék. A kártyák belső térköze legalább 32px, szükség esetén a lekerekített sarkok közelében nagyobb. A szövegek, ikonok és gombok biztonságos távolságra helyezkedjenek el a szélektől, ne kövessék a lekerekítés ívét, és ne kerüljenek túl közel a sarkokhoz.
- **Képek:** hangsúlyos, aszimmetrikus levélformájú lekerekítés (border-radius: 0 80px 0 80px), a jobb felső és bal alsó sarok lekerekített, a másik kettő szögletes. Nagyobb hero képeknél a lekerekítés akár 120px is lehet. A képek méretarányosan töltsék ki a rendelkezésre álló teret, a tartalmuk ne torzuljon, és a fontos részleteket ne vágja le a lekerekítés. Meleg, természetes fényű fotók, sok bőrtónussal, krém és bézs környezettel.
- **Űrlapmező:** fehér háttér, 1px halvány púder keret, 12px lekerekítés, fókuszra sötét zsályazöld (#50594A) keret, jól látható fókuszjelzéssel.
- **Ikonok:** vékony vonalas ikonkészlet (például Lucide vagy Phosphor Light), mély vagy sötét zsályazöld színben. A meleg barna dekoratív ikonokhoz használható, megfelelő kontraszttal.

Formavilág: A weboldal visszatérő vizuális motívuma az aszimmetrikus, levélformát idéző lekerekítés. A jobb felső és bal alsó sarkok hangsúlyosan lekerekítettek, míg a bal felső és jobb alsó sarkok szögletesek vagy csak enyhén lekerekítettek. Ez a forma jelenjen meg következetesen a gombokon, képeken és kártyákon, eltérő mértékű lekerekítéssel. A tartalom elhelyezésénél mindig elsődleges szempont az olvashatóság, a megfelelő belső térköz és a vizuális egyensúly. Mobilnézetben a lekerekítés mértéke arányosan csökkenthető, hogy ne vegyen el túl sok helyet a tartalomtól.

## Logó

A weboldalon a `logo/` mappában található, saját készítésű logókat kell használni. A logók megjelenését, betűtípusát, arányait és színeit változtatás nélkül meg kell őrizni, nem szabad újragenerálni vagy helyettesíteni.

- `logo.svg` / `logo.png` – világos háttérre
- `logo-feher.svg` / `logo-feher.png` – sötét háttérre
- `favicon.svg` / `favicon.png` – böngészőikon

Elsődlegesen az SVG-fájlokat kell használni. A logókat mindig méretarányosan, torzítás nélkül kell megjeleníteni.
