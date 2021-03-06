# VESM2-lokaverkefni (Dagbók í Wiki)
## Lokaverkefni (35%) 
Snúrustýrður bíll með fjarstýringu.

Í þessu einstaklingsverkefni áttu að nota Tinkercad til að gera frumgerð af fjarstýrðum bíl og fjarstýringu fyrir hann. Í þessari frumgerð notar þú að vísu snúru til að tengja saman bílinn og fjarstýringuna. Gert er ráð fyrir sjálstæðum vinnubrögðum í þessu lokaverkefni.

## Efnislisti
- 2 Arduino tölvur
- 2 DC mótorar
- 2 Servo mótorar
- LCD skjár
- Ultrasonic skynjari
- 4 Takkar eða 2 stilliviðnám
- H-Bridge
- 2 breadboard
- Slatti af snúrum og viðnámum
- Annað sem getur verið gagnlegt að hafa


### Samskipti
Bíllinn og fjarstýringin tala saman með I2C staðlinum.

### Bíllinn
Bíllin notar aðra Arduino tölvuna til að stjórna móturunum. DC mótorarnir eru fyrir afturdekkin og keyra bílinn áfram eða aftur á bak. Nota skal H-Bridge með DC móturunum. Servo mótorarnir sjá um að stýra stefunni á framdekkjunum. Hvað mótorarnir eiga að gera kemur frá fjarstýringunni. Ultrasonic skynjarinn er svo framan á bílnum og hefur það hlutverk stoppa DC mótorana ef bíllinn er innan við 50cm frá einhverju, þessa mælingu þar svo að senda til fjarstýringarinnar.

### Fjarstýringin
Hin Arduino tölvan er notuð sem fjarstýring. Við hana þarf að tengja 4 takka (hægri/vinstri/áfram/bakka) eða 2 stilliviðnám. Fjarstýringin er líka með LCD skjá en á honum á að birta fjarlægðina sem er mæld með Ultrasonic skynjaranum á bílnum.

### Hönnun 
Notaðu TinkerCad og/eða Inkscape til að hanna og útfæra umgjörð fyrir fjarstýringuna og bílinn (e. body). Það þarf m.a að hanna DC mótor, huga að að rými fyrir íhluti og tengingar. Það þarf ekki að hanna dekkin sjálf (það má gera ráð fyrir að þau séu tilbúin). Frjáls útfærsla að öðru leyti.

## Verkefnaskil
Haltu utan um verkefnið á github, þar á að vera:
- Dagbók, hvað gerðir þú og hvenær.
  * Svar: [Dagbók](https://github.com/Davygod/VESM2-lokaverkefni/wiki)
- Kóðinn af báðum Arduino tölvunum.
  * Svar: [Kóðinn](https://github.com/Davygod/VESM2-lokaverkefni/blob/master/Lokaverkefni2.ino)
- Hlekkur á Tinkercad teikninguna af rásunum (Muna að gera teikninguna Public).
  * Svar: [Teikning](https://www.tinkercad.com/things/4rYNnPmun6f-copy-of-arduino-car-2wd/editel)
- Hönnunarteikningar af bíl og fjarstýringu. Ein teikning með íhlutum (Arduino, skynjarar mótorar osfrv) og önnur án íhluta (til prentunar)
  * Svar: [Teikning með íhlutum](https://github.com/Davygod/VESM2-lokaverkefni/blob/master/Lokaverkefni-VESM2%20(3).stl) og [teikning án íhluta](https://github.com/Davygod/VESM2-lokaverkefni/blob/master/Lokaverkefni-VESM2%20(5).stl)


## Námsmat
1. Uppsetning í Tinkercad (Circuits) (20%)
  - 0% Uppsetning stórlega gölluð eða hana vantar.
  - 10% Uppsetningin virkar en er ósnyrtileg og erfitt að átta sig á hvað tengist hverju. Mikilvæga hluti vantar í uppsetninguna.
  - 20% Uppsetningin er snyrtileg og skýr til aflestrar. Notaðir eru mismunandi litir á víra og skynsamleg notkun á beygjum á þeim.

2. Kóði og virkni (50%)
   
   Gefið er í heilu og hálfu fyrir hvern lið.
   1. Bíll (30%)
      - Bíllinn getur beygt til hægri og vinstri (5%).
      - Skynjari sendir fjarlægðarupplýsingar (5%).
      - Hægt að keyra bíl áfram og afturábak (10%).
      - DC Mótorar hægja á sér áður en þeir skipta um átt (10%).
   
   2. Fjarstýring og samskipti (20%)
      - LCD sýnir fjarlægðarmælinguna frá bílnum (5%).
      - Hægt er að stjórna hraða og átt (áfram/bakka) með fjarstýringu (7%).
      - Hægt er að beygja (vinstri/hægri) bílnum með fjarstýringu (8%).

3. 3D hönnun  (30%)
   -  0% Vantar eða stórlega gölluð.
   - 10% Hönnun er gölluð eða ábótavant að nokkru leyti.
   - 20% Hönnun er uppfyllt að mestu leyti.
   - 30% Hönnun er góð, lögun umgjarðar fellur vel að fjarstýringu og bíl, allir íhlutir og skynjarar falla vel að hönnun og eru tengdir, rými fyrir Íhluti og skynjara er ekki of rúmt og það eru ekki göp, tengingar og samsetning er framkvæmanleg útfrá hönnun.
   
## Heimildir
1. https://www.tinkercad.com/things/4KfjPqZDUAF-arduino-car-2wd
2. https://www.instructables.com/id/motor-car-toy-with-arduino-uno-and-3dprinting/
3. https://www.tinkercad.com/things/3JTrjo0oj0s-copy-of-arduino-uno-casing-with-lcd-push-breadboard-space-and/edit
4. https://www.google.com/search?ei=yySwXs-sJa671fAPl4qP0AQ&q=using+servo+motor+for+steering+arduino+with+arduino+buttons&oq=using+servo+motor+for+steering+arduino+with+arduino+buttons&gs_lcp=CgZwc3ktYWIQAzoECAAQRzoICCEQFhAdEB46BQghEKABOgcIIRAKEKABOgQIIRAVUPErWIdZYP5ZaABwAngAgAGlAYgBohKSAQQ2LjE1mAEAoAEBqgEHZ3dzLXdpeg&sclient=psy-ab&ved=0ahUKEwiPvs_rs5rpAhWuXRUIHRfFA0oQ4dUDCAw&uact=5#kpvalbx=_6ySwXrTeMe6h1fAP68aK8Ao28
