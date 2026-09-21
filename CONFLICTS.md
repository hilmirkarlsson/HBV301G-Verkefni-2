# Árekstrar milli hagsmunaaðila

## Mæla haldtölu á móti gögnin fara ekki neitt

- **Árekstur:** Þróunarteymið þarf að vita hvort fólk heldur áfram að nota appið, því [BREQ-1][BREQ-1] segir að 40% nýrra notenda eigi enn að skrá æfingu í viku mánuði eftir að þeir byrja. En [C-2][C-2] segir að öll gögn séu í símanum, enginn server, og að gögnin fari ekki neitt. Ef ekkert fer úr símanum veit teymið ekki hvort 40% næst.
- **Hagsmunaaðilar:** Þróunarteymi (viðskiptavinur) og lyftari (notandi), sjá [STAKEHOLDERS.md](STAKEHOLDERS.md).
- **Orsök:** Teymið vill vita hvort appið virkar, því það er talan sem segir hvort það lifir ([SDS][SDS] segir að árangur mælist í þessu). Lyftari vill að æfingarnar hans séu hans eigin og fari ekkert ([BRG-1][BRG-1], [QA-2][QA-2]). Til að mæla þarf eitthvað að fara úr símanum, en til að vernda gögnin má ekkert fara.
- **Tegund:**
  - [ ] Viðfangsefnaárekstur (*subject matter conflict*)
  - [ ] Gagnaárekstur (*data conflict*)
  - [x] Hagsmunaárekstur (*interest conflict*)
  - [x] Gildisárekstur (*value conflict*)
  - [ ] Tengslaárekstur (*relationship conflict*)
  - [ ] Skipulagsárekstur (*structural conflict*)

  Þetta er hagsmunaárekstur því teymið vill mælinguna og notandi vill friðhelgi. Hann er líka gildisárekstur, því annar leggur áherslu á að safna gögnum og hinn á að safna sem minnstu vegna persónuverndar.

- **Úrlausn:** Skapandi lausn (*creative solution strategy*). Appið mælir bara **nafnlausa talningu** og notandi kveikir sjálfur á henni, hún er valfrjáls. Ekkert auðkenni og engin æfingagögn fara úr símanum, bara að einhver skráði æfingu í þessari viku. Þetta brýtur ekki BRG-1, sem bannar bara að afhenda gögn án skýrs samþykkis notanda. En C-2 þarf að breytast aðeins: „enginn server fyrir gögn notandans“ í stað „enginn server“.

  Rökstuðningur: Skapandi lausn leitar að því sem báðir þurfa í raun. Teymið þarf ekki gögnin sjálf, það þarf töluna um hversu margir halda áfram. Lyftari þarf ekki að vera án allra mælinga, hann þarf að æfingarnar hans séu hans. Talning án auðkennis gefur báðum það. Hinar leiðirnar henta verr:
  - Ákvörðunarleið lætur annan aðilann tapa. Tafla 6-3 í W&B (bls. 116) lætur viðskiptavininn ráða, en þar sem teymið er sjálft viðskiptavinurinn og BRG-1 er okkar eigin regla værum við þá að brjóta hana.

  Áhætta: Þeir sem kveikja á talningu eru líklega þeir sem nota appið mest, þannig að talan getur orðið hærri en raunverulega haldtalan.


[BREQ-1]: https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/business_requirements.md#breq-1
[C-2]: https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/constraint.md#c-2
[BRG-1]: https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/business_rule.md#brg-1-notendagögn-eign-notanda
[QA-2]: https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SRS/quality_attribute.md#qa-2-persónuvernd
[SDS]: https://github.com/hilmirkarlsson/HBV301G-Verkefni-1/blob/v1.0/SDS.md
