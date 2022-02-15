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
# Pedalaren switch-a
![36a0206d26f03fe1e3e172fcc9c9e-1678372](https://user-images.githubusercontent.com/99732982/154102945-45a3926a-cf34-47ce-bc08-192d143b5e8d.gif)
# Etapak
![big-muff-pi-v3-circuit-stages](https://user-images.githubusercontent.com/99732982/154099204-7d13a2d3-100c-4f80-a569-d0813b077eab.png)
# Pedalaren eskema
![big-muff-pi-v3-bias](https://user-images.githubusercontent.com/99732982/154100001-9d39c031-3fd7-4cbd-97db-6f5c30f9b89b.png)
# 
