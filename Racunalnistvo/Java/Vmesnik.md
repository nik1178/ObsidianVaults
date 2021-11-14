# Vmesnik (Interface)
- Objekt v [[Java|Javi]]
- z vmesnikom podamo, kaj morajo objekti znati
- Vmesnike je seznam deklaracij [[Metoda|metod]], ki so vedno samo abstraktne metode in zaradi tega ne rabimo pri deklaraciji napisati besede abstract
- Abstraktne metode imajo samo deklaracijo in so brez telesa
- Vmesnik deklariramo z besedo interface `public interace ImeVmesnika {...}`
- Razred ustreza oz. zadošča vmesniku, kar pomeni, da mora ta razred vsebovati vse metode tega vmesnika. Če ne vsebuje vseh metod, ne bo deloval, razen v primeru, da je abstraktni razred
- Vmesniki lahko podedujejo več vmesnikov hkrati, kar razredi ne morejo (public interace `Vmesnik extends Vmesnik2, Vmesnik3 {...})`
- Razred lahko ustrza več vmesnikom, vendar mora vsebovati metode vseh teh vmesnikov `public class Razred implements Vmesnik1, Vmesnik2{...}`
- Razred lahko tudi naenkrat deduje nadrazred in ustreza vmesnikom 
`public class Razred extends Razred2 implements Vmesnik1, Vmesnik2 {...}`

## Primerjava [[Abstraktni razred|abstraktnega razreda]] in [[Vmesnik#Vmesnik|vmesnika]]
### Podrazred abstraktnega razreda
- podeduje [[Spremenljivka|spremenljivke]] in metode razreda
- dodatno deklarira nove [[Spremenljivka|spremenljivke]] in metode. V primeru, da nam katera od podedovanih metod ne ustreza, jo lahko redefiniramo ("povozimo")
### Razred, ki zadošča vmesnikom
- Deklarira vse metode, ki so deklarirane v vmesnikih
- Lahko uporablja statične [[Spremenljivka|spremenljivke]], ki so definirane v vmesnikih

## Vmesnik kot tip
- Definiramo lahko lokalno [[Spremenljivka|spremenljivko]], katere tip je vmesnik 
`Vmesnik a = new Razred();` V tem primeru mora ta razred ustrezati temu vmesniku, da to deluje
- Ne moremo narediti tega: `Vmesnik a = new Vmesnik();`
