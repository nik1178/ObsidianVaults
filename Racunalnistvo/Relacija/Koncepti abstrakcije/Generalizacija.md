## Generazlizacija
- Posameznim tipom se priredo splošnejši tip na višjem nivoju

```mermaid
graph BT
0(Podtip entitete:)
Zaposlen & Študent & Upokojenec -->|je| občan
0---1(Posplošen tip:)
```
- Vpeljemo razmerje "JE" med elementarnimi tipi in posplošenim tipom na všiji ravni. Posplošeni tip lahko predstavlja elementarne in druge posplošene tipe
- Značilno je dedovanje - Lastnosti posplošenega tipa se dedujejo po hierarhiji navzdol


```mermaid
flowchart BT
	subgraph 1
		direction TB
		EMŠO---naslov--- Ime--- Priimek
	end
	subgraph 4
	direction LR
		Občan---1
	end
	subgraph 5
	direction LR
		Zaposlen---2
	end
	subgraph 2
		direction TB
		Sifra_organizacije --- poklic --- sifra_delavnega_mesta
	end
	Zaposlen-->Občan
	
```
- Po dednem pravilu ima ZAPOSLEN poleg svojih lastnosti še vse lastnosti tipa OBČAN, nima pa nekaterih svojih atributov, ki se ne bi podedovali po hierarhiji navzdol
