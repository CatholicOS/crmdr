# Draft canonical IDs — Martyrologium Romanum (CRMDR working document)

Generated mechanically from the Latin texts (editio altera 2004, 'elaborazione' transcription,
corrected against the Vatican print where noted). **All IDs are drafts for committee review.**

## Scheme

`mr:MMDD-slug` — MMDD anchors the entry's placement in the editio altera 2004;
the slug is the Latin nominative lemma of the first-named subject, ASCII-folded,
lowercase, honorific-free (no sanctus/beatus). Each edition's actual entry number,
asterisk, and placement are per-edition attributes, not part of the identity.

Rules applied, in order:
1. Personal names extracted after the first sanctity marker (sancti/beatae/sanctorum...);
   genitive converted to nominative by declension rules + a curated irregular map.
2. Religious-name titles after a/de remain uninflected (teresia-a-iesu, ignatius-de-loyola).
3. Papal ordinals rendered as roman numerals (pius-x, clemens-i); non-papal regnal
   ordinals remain Latin adjectives (ludovicus-nonus).
4. Cognomento epithets appended (petrus-chrysologus, albertus-magnus).
5. Two named subjects: both joined (cosmas-et-damianus). Three or more, or explicit
   'et sociorum': first-named + et-socii (paulus-miki-et-socii).
6. Marian titles: maria + invocation (maria-de-lourdes, maria-de-guadalupe).
7. Christological/liturgical feasts: manual override slugs (see below).
8. Anonymous groups: class + number + place, mechanically (quadraginta-milites-sebastem).
9. Same-slug collisions within a day: the day's lead keeps the bare slug; numbered
   entries take the place of death; ordinals as last resort.

## Special identity decisions

**Feb 28/29**: the four leap-day elogia printed twice in both IT and LA editions carry
ONE identity each, anchored at 0229; the Feb 28 rows bear the same ID:
- mr:0229-hilarius (also at Feb 28, voce 4)
- mr:0229-oswaldus (also at Feb 28, voce 5)
- mr:0229-antonia-de-florentia (also at Feb 28, voce 6)
- mr:0229-augustus-chapdelaine (also at Feb 28, voce 7)

**Editio-altera-only entries** (no row in the CEI-based workbook):
- mr:0104-abrunculus — print entry 2*, absent from the CEI and from the Word transcription
- mr:0104-emmanuel-gonzalez-garcia — print entry 12*, absent from the CEI (Bl. M. González García, canonized 2016:
  status change with no ID change, as intended)

**Repaired source text**: the Word transcription's 3-20 v1 was truncated; the la cell was
restored from the print (Commemoratio sancti Archippi...). ID: mr:0320-archippus.

## Manual feast overrides (34)

- mr:0101-maria-dei-genetrix  (1/1 voce 1)
- mr:0103-nomen-iesu  (1/3 voce 1)
- mr:0106-epiphania-domini  (1/6 voce 1)
- mr:0125-conversio-sancti-pauli  (1/25 voce 1)
- mr:0202-praesentatio-domini  (2/2 voce 1)
- mr:0217-septem-fundatores-servorum-mariae  (2/17 voce 1)
- mr:0222-cathedra-sancti-petri  (2/22 voce 1)
- mr:0320-archippus  (3/20 voce 1)
- mr:0325-annuntiatio-domini  (3/25 voce 1)
- mr:0325-bonus-latro  (3/25 voce 2)
- mr:0531-visitatio-beatae-mariae-virginis  (5/31 voce 1)
- mr:0717-alexius  (7/17 voce 5)
- mr:0724-translatio-trium-magorum  (7/24 voce 13)
- mr:0728-martyres-thebaidis  (7/28 voce 3)
- mr:0805-dedicatio-basilicae-sanctae-mariae  (8/5 voce 1)
- mr:0806-transfiguratio-domini  (8/6 voce 1)
- mr:0815-assumptio-beatae-mariae-virginis  (8/15 voce 1)
- mr:0820-pius-x  (8/20 voce 9)
- mr:0822-maria-regina  (8/22 voce 1)
- mr:0908-nativitas-beatae-mariae-virginis  (9/8 voce 1)
- mr:0912-nomen-mariae  (9/12 voce 1)
- mr:0913-dedicatio-basilicarum-hierosolymis  (9/13 voce 3)
- mr:0914-exaltatio-sanctae-crucis  (9/14 voce 1)
- mr:0915-maria-perdolens  (9/15 voce 1)
- mr:1002-angeli-custodes  (10/2 voce 1)
- mr:1003-duo-ewaldi  (10/3 voce 7)
- mr:1101-omnes-sancti  (11/1 voce 1)
- mr:1102-omnium-fidelium-defunctorum  (11/2 voce 1)
- mr:1109-dedicatio-basilicae-lateranensis  (11/9 voce 1)
- mr:1118-dedicatio-basilicarum-petri-et-pauli  (11/18 voce 1)
- mr:1121-praesentatio-beatae-mariae-virginis  (11/21 voce 1)
- mr:1208-conceptio-immaculata-beatae-mariae-virginis  (12/8 voce 1)
- mr:1224-avi-iesu-christi  (12/24 voce 1)
- mr:1225-nativitas-domini  (12/25 voce 1)

## Anonymous groups — mechanical slugs, review recommended (39)

- mr:0114-monachi-raithi
  - *Incipit:* Commemorátio sanctórum monachórum, qui Raíthi et…
- mr:0205-plurimi-martyres-ponto
  - *Incipit:* In Ponto, commemorátio plurimórum sanctórum mártyrum…
- mr:0208-martyres-monachi-dii-constantinopolitani
  - *Incipit:* Commemorátio sanctórum mártyrum monachórum monastérii Dii…
- mr:0209-plurimi-martyres-alexandriae
  - *Incipit:* Item Alexandríæ, pássio plurimórum sanctórum mártyrum,…
- mr:0211-plurimi-martyres-numidia
  - *Incipit:* Commemorátio plurimórum sanctórum mártyrum, qui in…
- mr:0212-martyres-carthagine
  - *Incipit:* Carthágine, commemorátio sanctórum mártyrum Abitinénsium, qui,…
- mr:0219-monachi-martyres-palaestina
  - *Incipit:* Commemorátio sanctórum monachórum et aliórum mártyrum,…
- mr:0220-quinque-martyres-tyri
  - *Incipit:* Commemorátio beatórum quinque mártyrum, qui, sub…
- mr:0228-presbyteri-diaconi-plurimi-alexandriae
  - *Incipit:* Commemorátio sanctórum presbyterórum, diaconórum et aliórum…
- mr:0306-quadraginta-duo-martyres-syria
  - *Incipit:* In Sýria, pássio sanctórum quadragínta duórum…
- mr:0309-quadraginta-milites-sebastem
  - *Incipit:* Apud Sebástem in Arménia, pássio sanctórum…
- mr:0330-plurimi-martyres-constantinopoli
  - *Incipit:* Commemorátio sanctórum plurimórum mártyrum, qui Constantinópoli,…
- mr:0405-centum-undecim-viri-novem-mulieres-martyres
  - *Incipit:* Item, commemorátio centum úndecim virórum ac…
- mr:0405-martyres-regiis
  - *Incipit:* Régiis in Mauretánia, pássio sanctórum mártyrum,…
- mr:0407-ducenti-milites-martyres-sinope
  - *Incipit:* Sinópe in Ponto, sanctórum ducentórum mílitum…
- mr:0509-martyres-trecenti-decem-perside
  - *Incipit:* In Pérside, sanctórum mártyrum trecentórum et…
- mr:0516-quadraginta-quattuor-monachi-palaestina
  - *Incipit:* In Palæstína, pássio sanctórum quadragínta quáttuor…
- mr:0521-martyres-alexandriae
  - *Incipit:* Commemorátio sanctórum mártyrum utriúsque sexus, quos…
- mr:0523-martyres-cappadocia
  - *Incipit:* Commemorátio sanctórum mártyrum, qui in Cappadócia…
- mr:0523-martyres-mesopotamia
  - *Incipit:* Item commemorátio sanctórum mártyrum, qui eódem…
- mr:0524-triginta-octo-martyres-philippopoli
  - *Incipit:* Commemorátio sanctórum trigínta et octo mártyrum,…
- mr:0708-monachi-constantinopoli
  - *Incipit:* Constantinópoli, pássio sanctórum monachórum Abrahamitárum, qui,…
- mr:0801-septem-fratres-martyres-antiochiae
  - *Incipit:* Commemorátio passiónis sanctórum septem fratrum mártyrum,…
- mr:0809-martyres-constantinopoli
  - *Incipit:* Constantinópoli, commemorátio sanctórum mártyrum, qui, cum…
- mr:0810-martyres-alexandriae
  - *Incipit:* Commemorátio sanctórum mártyrum, qui Alexandríæ in…
- mr:0814-octingenti-martyres-hydrunti
  - *Incipit:* Hydrúnti in Apúlia, beatórum fere octingentórum…
- mr:0830-sexaginta-martyres-coloniae-sufetanae
  - *Incipit:* Commemorátio sanctórum sexagínta mártyrum, qui, Colóniæ…
- mr:1005-martyres-treviris
  - *Incipit:* Tréviris in Gállia Bélgica, commemorátio sanctórum…
- mr:1010-septem-martyres-presbyteri-septam
  - *Incipit:* Apud Septam in Mauritánia Tingitána, pássio…
- mr:1012-martyres-confessores-quattuor-sexaginta-africa
  - *Incipit:* Commemorátio sanctórum mártyrum et fídei confessórum…
- mr:1021-virgines-coloniam-agrippinam
  - *Incipit:* Apud Colóniam Agrippínam in Germánia, commemorátio…
- mr:1113-martyres-africa
  - *Incipit:* In Africa, commemorátio sanctórum mártyrum hispanórum…
- mr:1115-viginti-martyres-hippone-regio
  - *Incipit:* Hippóne Régio in Numídia, sanctórum vigínti…
- mr:1119-mulieres-virgines-viduae-quadraginta-martyres-heracleae
  - *Incipit:* Heracléæ in Thrácia, sanctárum mulíerum, vírginum…
- mr:1206-martyres-africa
  - *Incipit:* In Africa, commemorátio sanctórum mártyrum, témpore…
- mr:1216-plurimae-virgines-africa
  - *Incipit:* Commemorátio plurimárum sanctárum vírginum, quæ, in…
- mr:1217-quinquaginta-milites-eleutheropoli
  - *Incipit:* Eleutherópoli in Palæstína, pássio sanctórum quinquagínta…
- mr:1222-triginta-martyres-romae
  - *Incipit:* Romæ via Labicána in cœmetério ad…
- mr:1222-quadraginta-tres-monachi-raithi
  - *Incipit:* In Raíthi regióne in Ægýpto, sanctórum…

## Collision resolutions (36)

- 1/27 voce 2: iulianus → place sorae
- 1/27 voce 3: iulianus → place cenomanum
- 2/4 voce 5: aventinus → place castelloduni
- 2/4 voce 6: aventinus → place trecis
- 2/13 voce 4: stephanus → place lugduni
- 2/13 voce 5: stephanus → place reate
- 4/1 voce 6: hugo → place gratianopoli
- 4/1 voce 7: hugo → place cisterciensi-bonae
- 4/3 voce 4: ioannes → place neapoli
- 4/3 voce 9: ioannes → place pinnae
- 4/8 voce 3: dionysius → ordinal 2
- 4/8 voce 5: dionysius → place alexandriae
- 4/17 voce 9: robertus → place casae
- 4/17 voce 10: robertus → place molismensi
- 4/23 voce 1: georgius → lead-bare 
- 4/23 voce 6: georgius → place suellis
- 7/3 voce 2: anatolius → place laodiceae
- 7/3 voce 6: anatolius → place constantinopoli
- 8/7 voce 4: donatus → place aretii
- 8/7 voce 7: donatus → place vesontione
- 9/13 voce 8: amatus → place vosegos
- 9/13 voce 10: amatus → place broili
- 9/18 voce 3: ferreolus → place galliae-viennensi
- 9/18 voce 6: ferreolus → place lemovici
- 10/9 voce 5: domninus → place iuliam
- 10/9 voce 8: domninus → place tiferni-tiberini
- 10/23 voce 3: ioannes → place perside
- 10/23 voce 7: ioannes → place syracusis
- 11/11 voce 2: menna → place mareotidem
- 11/11 voce 4: menna → place samnii
- 11/17 voce 2: gregorius → place neocaesareae
- 11/17 voce 7: gregorius → place turonis
- 11/17 voce 11: hugo → place nucariae
- 11/17 voce 12: hugo → place lincolniae
- 11/21 voce 3: maurus → place parentii
- 11/21 voce 6: maurus → place caesenae

## Known caveats for the committee

- Rare genitives with no safe rule remain in genitive form (single-occurrence Greek
  and Germanic names); they are still unique and stable, but not always nominative.
- Surname/epithet ambiguity for tokens in -i is resolved by corpus frequency; a
  1-in-corpus Latin epithet may remain unconverted while surnames are protected.
- The namespace prefix `mr:` and the anchor-edition choice are placeholders for
  committee decision; changing either is a mechanical rewrite.
