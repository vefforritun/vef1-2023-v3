# Vefforritun 1, 2022: Verkefni 3, CSS #1

## Markmið

- Tengja CSS við HTML.
- Aðlaganir á HTML fyrir CSS.
- Notkun á grunn CSS með box model; visual formatting model og; letri og litum.

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2023-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2023-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2023-v4) setur upp útlit (e. layout).
- [Verkefni 5](https://github.com/vefforritun/vef1-2023-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2023-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Verkefnið

Verkefnið er framhald af [verkefni 2](https://github.com/vefforritun/vef1-2023-v2), nýtir það efni sem uppsett er í því, og fylgir þeirri verkefnalýsingu. Leyfilegt er að nota [sýnilausn að verkefni 2](https://github.com/vefforritun/vef1-2023-v2-synilausn), sem gefin verður út föstudaginn 8. september.

Nú skal bæta við einföldu útliti á efnið með CSS. Allt útlitið skal vera í `./styles.css` og **allar** HTML skrár skulu vísa í það.

## Útlit

Fyrirmynd að útliti er í `fyrirmynd/` möppu. Öll skjáskot eru tekin í `1000px` breiðum Firefox vafra.

Gera má ráð fyrir að það verði að bæta við auka elementum við lausn/sýnilausn til að geta náð fram útliti.

Þar sem allt útlit skal útfæra í einni CSS skrá, skal huga að cascade og erfðum, þó er fullkomlega eðlilegt að endurtaka eigindi, en t.d. fyrir málsgreinar (`<p>`) þarf aðeins að taka fram einu sinni hvert margin þeirra er. Fyrir útlit sem notar „box“ er hægt að útfæra einu sinni og endurtaka þrisvar sinnum.

### Almennt

Gefið er `styles.css` skjal með grunn að lausn.

Almennt skal gilda:

- Nota skal gefið „reset“ (merkt sérstaklega), það má ekki fjarlægja.
- Nota skal leturgerðina Lora frá Google fonts. Sækja þarf bæði regular (þyngd `400`) og bold (þyngd `700`).
- Gefin er stærð á letri sem `16px` (sem merkir að `1rem == 16px`), því skal ekki breyta. Í framhaldi af lýsingu er `eitt bil = 1rem`, `hálft bil = 0.5rem` o.s.fr.
- Gefin er hjálparklasi `.sr-only` sem skal setja á `Beint í efni` tengil.
- Aðeins skal nota `px` í grunnleturstærð og á `border` skilgreiningar, annars skal nota hlutfallslegar einingar (`em`, `rem`, eða `%`)
- Allt efni (málsgreinar, myndir, form element) skal hafa eitt bil fyrir neðan sig.
- Allir litir: `#ffe7ae`, `#2f0505` `#fff1cf`, `#fff9ee`
- CSS skal vera án villna og **viðvarana** þegar keyrt í gegnum [CSS validator](https://jigsaw.w3.org/css-validator/), einnig hægt að keyra gegnum W3C Validator extension.

Allt sem gildir í verkefni 2 gildir áfram í þessu verkefni.

### Haus, valmynd, meginmál og fótur

Setja skal aukalega upp þ.a.:

- Haus notar bakgrunnslitinn `#2f0505` sem teygir sig alveg út í alla breidd vafra, texti innan haus sé miðjaður og eitt bil á alla kanta. Fyrir neðan sé `8px` border með litinn `#ffe7ae`.
- Allt efni sé að hámarki `900px` breitt og sé miðjað í vafra.
- Valmynd er beint fyrir neðan haus með eitt bil á alla kanta með bakgrunnslit `#fff9ee``.
- Efni í valmynd flæði frá vinstri til hægri og sé miðjað.
- Valin síða í valmynd á að vera feitletruð og ekki með undirlínu.
- Fótur (`<footer>`) hafi bakgrunnslitinn `#2f0505` með `8px` border með litinn `#ffe7ae` fyrir ofan.
- Eitt bil sé alltaf milli meginmáls og fóts.
- Efni í fóti sitji hlið við hlið með bilum milli fyrirsagnar og efnis.

Þegar útlit er sagt nota box:

- Efni er með tvö bil fyrir neðan sig og `2px` border með litinn `#ffe7ae`.
- Efni í boxum raðist tvö saman hlið við hlið

### Forsíða

Opnunartími, um okkur, matseðill og panta séu að nota box.

Vinsælir réttir séu að nota box.

### Um

Eitt bil frá fyrirsögn að efni. Listi af starfsfólki sé að nota box.


### Pöntunarsíða

Utan um hvert svæði í pöntun sé `1px` border með litinn `#ffe7ae`. Svæðin séu að nota box.

Setja skal hálft bil af lárréttu `padding` í `input` og fyrir tjékkbox.

### Matseðill

Tafla fylli út í allt efnissvæði og hafi vinstri jafnaðan texta.

Fyrsta og hver oddatölu röð sé lituð með `#ffe7ae`.

### Takmarkanir

Aðeins skal nota eftirfarandi eigindi, og ef tekið fram, viðeigandi gildi:

- `background-color`
- `border` og nánari skilgreiningar
- `border-spacing: 0;`
- `box-sizing`
- `color`
- `display: block;`, `display: inline-block;`
- `font-family`
- `font-size`
- `font-weight`
- `list-style: none;`
- `margin` og nánari skilgreiningar
- `padding` og nánari skilgreiningar
- `width`, `min-width`, `max-width`, `min-height`
- `text-align`
- `text-decoration`
- Þau eigindi notuð í `.sr-only` og ekki tiltekin hér ætti ekki að nota í annað.

Ekki þarf að huga að skalanleika (síðan þarf ekki að líta vel út í undir `800px` skjá).

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo.

## Mat

- 20% – Snyrtilega uppsett og gilt CSS.
- 20% – Aðeins leyfileg eigindi og gildi notuð.
- 60% – Útlit skv. fyrirmynd.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 4. september 2023.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 14. september 2023.

Skilaboð skulu innihalda:

- zip skrá með öllum skrám _eða_ hlekkur á GitHub.
- slóð á verkefni keyrandi á Netlify sem athugasemd („Add comment“ eða „Bæta við athugasemd“ á skilaskjá í Canvas).

## Einkunn

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ef stórt mállíkan (LLM, „gervigreind“, t.d. ChatGTP) er notað til að skrifa part af lausn skal taka það fram. [Sjá nánar á upplýsingasíða um gervigreind hjá HÍ](https://gervigreind.hi.is/).

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.1
