# Software Requirements Specification (útgáfa fyrir verkefni 2)
## Númer teymis og höfundar
Teymi 1: Hilmir Karlsson og Silja Ástudóttir

## Heiti kerfis
Settið

## 1. Inngangur

### 1.1 Gildissvið (Scope)
Settið er einfalt app fyrir fólk sem lyftir. Notandi skráir settin sín á meðan æfingin stendur yfir, fylgir plani sem segir hvað á að gera í dag og sér hvort þyngdirnar eru að hækka. Helstu markmið vörunnar eru að fólk haldi áfram að nota appið (BREQ-1, 40% haldtala) og að nýjum notendum fjölgi án auglýsinga (BREQ-2). Þetta skjal nær yfir hagsmunaaðila, notendahópa og einn árekstur. Kröfur kerfisins sjálfs eru í SRS í [Verkefni 1](https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/SRS.md).

### 1.2 Tilvísanir
- IEEE 29148 staðall
- Wiegers og Beatty, *Software Requirements*, 3. útg.
- Pohl, *Requirements Engineering – Fundamentals, Principles and Techniques*, 2. útg. 2025, kaflar 29 og 30
- [SRS úr Verkefni 1](https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/SRS.md), útgáfa v1.0

## 2. Lýsing á hagsmunaaðilum og notendahópum

Helstu hagsmunaaðilar eru lyftari (notandi) og þróunarteymi (viðskiptavinur). Notendahóparnir eru fjórir: byrjandinn, ráfarinn, sá sem sér engar framfarir og methafinn. Persónan Aron Bjarkason er úr hópnum methafinn.

[Hagsmunaaðilar og notendahópar](STAKEHOLDERS.md)

## 3. Greining á mögulegum árekstrum og tillögu að úrlausnum

Við greindum einn árekstur: þróunarteymið þarf að mæla haldtöluna (BREQ-1) en gögnin eiga ekki að fara úr símanum ([C-2](https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/constraint.md#c-2)). Þetta er hagsmuna- og gildisárekstur. Við leggjum til nafnlausa talningu sem notandi kveikir sjálfur á (skapandi lausn).

[Árekstrar og úrlausnir](CONFLICTS.md)

## 4. Verkaskipting og ígrundun

Hilmir tók CONFLICTS.md, README.md, SRS.md og Vinnuferli.md, Silja tók STAKEHOLDERS.md. Við rýndum Pull Request hvort hjá öðru.

[Verkaskipting](Vinnuferli.md#verkaskipting) · [Ígrundun](Vinnuferli.md#ígrundun)

## 5. Vinnuferli

Verkefnið er unnið á Kanban borði. Hvert issue fær sitt branch, breytingar fara í Pull Request sem hitt okkar rýnir og samþykkir, og höfundur merge-ar það við `main`. Gagnsæisyfirlýsing um notkun gervigreindar er líka í Vinnuferli.md.

[Vinnuferli](Vinnuferli.md)
