# Izjeme
- so dogodki, ki se zgodijo, ko gre nekaj narobe
- program se prekine, uporabnik dobi obvestilo
- Primeri:
	- ArithmeticException
	- ArrayIndexOutOfBoundsException
	- StringIndexOutOfBoundsException
	- NullPointerException
## Lovljenje izjem
#### Try-Catch

```
try{
	//koda
} catch (Exception e){
	//catch blok
} final {
	//se vedno izvede
}
```
Proba izvesti ukaze v `try`. Če pride do napake, izvrši ukaze v `catch`. Ukazi v `final` se vedno izvedejo.
- ##### Več izjem:

```
try{

} catch (ExceptionTipa1 e1){

} catch (ExceptionTipa2 e2){

} catch (ExceptionTipa3 e3){

} final {

}
```

#### Throws
[[Metoda|Metodi]] dodamo `throws + "tip izjeme"` po oklepaju:
```
public static void metoda(spremenljivke) throws Izjema{}
```
## Hierarhija izjem
- Izjeme so razdeljene po hierarhiji
- višje kot je izjema, več izjem pokriva
- če uporabimo izjeme višjega nivoja, avtomatsko pokrijemo vse podrejene izjeme

## Izjeme
- Naj bi jih čim več lovili - uporabljali
- ščitijo pred malomarnim programiranjem in pred še bolj malomarnimi uporabniki
- če jih je preveč je program nepregleden
- delitev:
	- [[Izjeme#Nepreveljive|nepreveljive]]
	- [[Izjeme#Preverljive|preverljive]]

#### Nepreveljive

- So vse izjeme, ki so naslednice razredov `java.lang.Error` in `java.lang.RuntimeException` ter njunih podrazredov
- ni jih nujno loviti
- če jih lovimo, se program izvede dalje
- če jih ne lovimo, jih lovi navidezni stroj in program se ustavi z obvestilom

#### Preverljive
- so vse ostale izjeme
- nujno jih je loviti
- primer: Delo z datotekami - IOException
- Če želimo posredovati izjemo klicoči metodi, uporabimo ukaz [[Izjeme#Throws|throws]]

