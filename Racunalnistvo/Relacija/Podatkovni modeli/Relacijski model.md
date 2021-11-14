## Relacijski model

### Elementi relacijskega modela
###### Relacija
Celotna tabela vrednosti

###### n-terka
Vrstica ali opis (je ?atomarna? - ni je možno razstavljati)

###### Atribut
Stolpec ali polje

###### Relacijska shema
R(A1, A2, ..., An)
npr.: ŠTUDENT(Ime, Vpis_stLetnik, Spol)

###### Domena
Vrednost atributov

Ime|Vpis_st|Letnik|Spol
---|-------|------|----
Jernej|12345|1|M
Mitja|12346|2|M
Vanja|12347|1|Ž

### Lastnosti
- matematičen koncept relacije
- preprost
- podatki predstavljeni kot zbirka relacij
- kot tabela
- imamo podmnožico atributov, ki enolično določajo n-terko v shemi; pravimo ji [[Modeliranje podatkov#Ključ|ključ]] relacije
- vsaka [[Relacijski model#Relacija|relacija]] ima lahko več kandidatov, vender le en izberemo za ključ
- S ključem iščemo podatke

#### Operacije med relacijami
- operacije za iskanje
- operacije za ažuriranje
- obe skupini tvorita [[Povpraševalni jezik|povpraševalnik jezik]]

![[Povpraševalni jezik]]

#### Operacije za ažvriranje relacij:
- dodajanje vrstic v relacijo
- brisanje vrstic (najprej izbor, nato brisanje)
- spreminjanje komponent

![[Relacijska algebra]]