# E-R model (entitetno-relacijski)
- model je naslednik [[Podatkovni modeli#Klasični|klasičnih modelov]]
- zelo široka uporaba
- združuje lastnosti [[Mrežni podatkovni model|mrežnih]] in [[Relacijski model|relacijskih modelov]]
- slabost: ni standardizirane predstavitve
- osnove modela:
	- matematična definicija množice in [[Relacijski model#Relacija|relacije]]
- elementi modeliranja;
	- entiteta, [[E-R model#atribut|atribut]], povezava-relacija, lahko tudi tip entitete


Državljan|||--->Tip entitete 
-|-|-|-
Ime|Spol|Poklic| --->atributi
Janez|M|Inženir|\|
Marko|M|Delavec|\|-->entitetna množica
Ana|Ž|Trajnica|\|
^|^|^ Vrednost atributa

## Definicije pojmov
###### Entiteta
- Napisano DIY:
	- Tabela, v katero shranjujemo podatke I guess kinda, ampak to velja samo pri E-R modelu. Pri relacijskem modelu je [[Relacijski model#Relacija|relacija]] tabela in entiteta vrstica I think
###### atribut
Je funkcija, ki tipu entitete priredi množico pripadajočih vrednosti atributa
###### enovrednostni atribut
za posamezen primerek entitete nastopa samo ena možna vrednost (npr. datum rojstva pri občanu)
###### večvrednostni atribut
Pri nekaterih atributih lahko pri posamezni entiteti nastopa več vrednosti (npr. atributi poklic ima lahko pri posameznih primerkih več vrednosti, en primerek ima lahko več različnih poklicev)
###### entitetni diagram
Je orodje za modeliranje podatkov, ki prikazuje povezave (odnose) med različnimi kategorijami podatkov v okviru obravnanega sistema

![[Postopek oblikovanja entitetnega modela]]

##### Z E-R modelom opišemo podatkovni vidik strukturne analize

![[Zapis E-R diagrama]]
![[Primer E-R modela]]
![[Grafični simboli za predstavitev E-R modela]]
![[Modeliranje]]
![[Normalizacija]]