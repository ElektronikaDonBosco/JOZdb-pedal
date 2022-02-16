# BIG JOZ 6D pedala:
Guitarraren señalea distortsionatzen duen pedala eta seinale hori irakurtzen duen arduino neurgailua.
# Zertan datza proiektuak?
Gure proiektua musikaren munduan murgildua dago. Erronka honetan, bi helburu nagusi genituen:

Batetik Gitarraren seinalea distortsionatuko zuen pedal bat sortu behar genuen, zehazki Big Muff Pi pedalaren bertsio bat, honen funtzionamendu basikoez gain, 2p3t switch bat ezarri genion. Honek 18 diodo gehitzen zizkion, (bata bestearekin binaka jarriak) bikote bakoitzak, ezaugarri berezi bat gehitzen zion irteerako seinaleari. Irteeran distrotsio soinu egokia lortu genuen.

Bestetik, arduino bidez audioa neurtzeko proiektua genuen. Honek gure pedaletik ateratzen zen seinalea irakurtzen zuen eta 8X8-ko LEd matrzi batean plasmatzen zuen. 4 matrize genituen eta bakoitza kontrolatzeko txip berezi baten beharrean giñen.

# Funtzionamendua:  
Big Muff Pi pedala, gitarrarentzako eginda dagoen distortsio pedal bat da. Gure kasuan distortsio gehiago areagotzeko prozesuan 2p3t switch-a gehitu diogu. Honek diodoak gehitzen dizkio pedalari, eta hauen bidez distortsio efektu ezberdin gehiago gehitzen zaizkio. Pedal honek lau fase ditu, lehenengoa sarrerako seinalea amplifikatzean datza, sarrerako 200mV-ak 7Vra bihurtuz, hau guztia emisore komuneko amplifikagailua erabiliz. Bigarren etapa ebakitze etapa da. Lehen transistoreak emeki ebakitzen du uhina: distortsioa sortzen du eta seinalea iragazten du. Lehen ebaketa-transistorearen ondoren, bigarrenak berriro errepikatzen du prozesua, eta desitxuratutako seinalea fintzen du. 3. etapa tonu kontrola da pasabide altuko eta baxuko iragazkien konbinazio bat  da. Azkeneko etapa irteera etapa da, igorle arruntaren anplifikadorea da, tonu pasiboen bolumenaren galera berreskuratzen duena. Disortsioa guk nahi genuenean erabili ahal izateko switch pedala gehitu genion. Honek bypass bat bezela funtzionatu dezake eta gitarratik sartzen den seinalea modifikatu gabe sartu den bezela atera egiten du. Ordea, switch-a zanpatzean seinalea zirkuituan sartzen da eta distortxioa irteerako jackera eramaten du. Gure kasuan pedalaren switcha aparteko plaka batean jarri genuen PCB-a bi zatitan banatuz.
# Prototipoa

![WhatsApp Image 2022-02-15 at 17 11 37](https://user-images.githubusercontent.com/99732982/154102165-0605c63f-b076-4733-a46f-68bc28440ce5.jpeg)

Kaxa barruan sartu aurretiko argazkia.

![WhatsApp Image 2022-02-16 at 16 48 07](https://user-images.githubusercontent.com/99732982/154357264-396e1783-9072-4f28-81c2-1092b2ac93bb.jpeg)

kaxa barruan sartua:

# Pedalaren switch-a

![36a0206d26f03fe1e3e172fcc9c9e-1678372](https://user-images.githubusercontent.com/99732982/154102945-45a3926a-cf34-47ce-bc08-192d143b5e8d.gif)
# Etapak

![big-muff-pi-v3-circuit-stages](https://user-images.githubusercontent.com/99732982/154099204-7d13a2d3-100c-4f80-a569-d0813b077eab.png)

# Pedalaren eskema
![big-muff-pi-v3-bias](https://user-images.githubusercontent.com/99732982/154100001-9d39c031-3fd7-4cbd-97db-6f5c30f9b89b.png)

# Big Muff Pi Bias y respuesta de tono.

![bmp-waveforms](https://user-images.githubusercontent.com/99732982/154357549-c1768df8-41f2-4b1b-b35c-19b1d106a518.png)

Seinale Laranja: sarrerako seinalea da, proba honetarako gitarra motako seinale bat erabiltzen da, 1KHz, 200mVpp.

Seinale Beltza: Input Booster irteera da, bakarrik alderantzizko eta anplifikatutako sarrerako seinalea 9.6 aldiz (19.6dB).

Seinale Gorria: Clipping-en lehen etapako irteera da, aurreko seinalea 23 dBs handitzen da eta zabalera ± 0.6V-ra murrizten da. Sustain potentziometroa gehieneko balioari egokituta dago.

Seinale urdina: Clipping-en lehen etapako irteera da, aurreko seinalea 25 dBs anplifikatzen da eta zabalera ± 0.6V-ra murrizten da. Ondoz ondoko bi ebaketa-etapa egin ondoren, forma karratuagoa edo gogorragoa da.

Seinale Berdea: tonu-kontrolaren ondorengo irteera da, batez besteko posizioan finkatuta. Seinalea 13dBs inguruan arintzen da, 1KHz-ra mid scoop-a hor dagoelako eta forma pixka bat aldatzen delako.

Pink Signal: Big Muff Pi-aren irteera seinalea da. Aurreko seinalea 13dBs anplifikatzen da maiztasun-aldaketarik gabe. Bolumen-potentziometroa gehieneko balioari egokituta dago.

# Materialak:
-4 NPN transistore: BC239 edo baliokideak 2N5088, 2N5089, BC549C, SE4010, 2N5210, 2N5113: Q 1, Q 2, Q 3, Q 4.

-Siliziozko 4 diodo: 1N914 edo baliokidea 1N4148: d 1, D 2, D 3, D 4.

-3 Potentziometro 100K Lin: Sustain, Tono, Bolumen.

-5 Erresistentzia 10K: R 13, R 19, R 18, R 11 R 12.

-3 Erresistentzia 100K: R 20, R 16, R 3.

-3 Erresistentzia 470K: R 9, R 17, R 15.

-2 Erresistentzia 39K: R 2, R 8.

-2 Erresistentzia 150: R 21, R 10.

-2 Erresistentziak 15K: R 6.

-1 Erresistentzia 47K: R 14.

-1 Erresistentzia 100: R22.

-3.3K erresistentzia: R 4.

-1K erresistentzia: R 23.

-1 Erresistentzia 22K: R 5

-4 1uF kondentsadoreak: C 1, C 4, C 6, C 7.

-4 kondentsadore 100nF: C 5, C 13, C 3, C 2.

-3 kondentsadore 470pF: C 10, C 11, C 12.

-4nF Kondentsadorea: C 9.

-10nF Kondentsadore 1: C 8.
