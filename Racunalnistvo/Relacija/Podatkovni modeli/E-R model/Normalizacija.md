# Normalizacija
- Je tehnika s katero pridemo do neredundantnih podatkov
- Je tehnika, ki jo uporabljamo pri določanju podatkovnih potreb organizacije z namenom dosega take oblike, ki je primerna za raučunalniško hranjenje
- Podatkovna normalizacija omogoča prevedbo kompleksnega modela v množico bolj preprostih in bolj stabilnih podatkovnih struktur
- normalizirana strukture je fleksibilna, stabilna in lažja za vzdrževanje

```mermaid
flowchart TD
0[normalizirani podatki]-->|odprava ponavljajočih grup|1[1. normalizirana forma]
1-->|odprava odvisnosti od dela ključa|2[2. normalizirana forma]
2-->|odprava tranzitivne odvisnosti|3[3. normalizirana forma]