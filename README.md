# Matador Spil

Dette er et Matador-spil udviklet i Java. Spillet er en digital version af det klassiske brætspil, hvor spillere kan købe ejendomme, bygge huse, og forsøge at ruinere deres modstandere ved at få dem til at lande på deres ejendomme. Formålet med spillet er at blive den rigeste spiller og få de andre spillere til at gå bankerot.

## Funktioner

- Opret flere spillere og tilpas navne
- Køb ejendomme og byg huse/hoteller
- Håndtering af pengestrøm (indkomst, leje, bøder mv.)
- Brug af terninger til at bevæge sig på spillebrættet
- Spilgrænseflade med tekstbaseret brugerinput

## Skærmbilleder

![Skærmbillede af spil](path/to/screenshot.png) <!-- Opdater med faktiske skærmbilleder -->

## Teknologier

- **Java** - Primært programmeringssprog til udviklingen af spillet
- **OOP (Objektorienteret programmering)** - For at opnå en modulær og struktureret kodebase
- **JDK** - Java Development Kit, version 11 eller nyere anbefales

## Kom godt i gang

For at få en lokal kopi af spillet op og køre, følg disse trin.

### Forudsætninger

- Installeret [Java JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) (version 11 eller nyere)
- En IDE som IntelliJ IDEA, Eclipse eller NetBeans

### Installation

1. Klon repository:
   ```bash
   git clone https://github.com/dinbrugernavn/MatadorSpil.git
   ```

2. Åbn projektet i din foretrukne Java-IDE.

3. Byg projektet ved hjælp af din IDE eller via kommandolinjen:
   ```bash
   javac -d bin src/*.java
   ```

4. Kør spillet:
   ```bash
   java -cp bin Main
   ```

## Spilbeskrivelse

Matador-spillet er et turbaseret økonomisk strategi-spil, hvor spillere skiftes til at kaste terninger og bevæge sig rundt på brættet. Afhængigt af hvilket felt en spiller lander på, kan de købe ejendomme, betale leje eller trække et kort fra bunken med "Chancekort".

### Spilregler:

- **Start**: Hver spiller starter med en vis sum penge.
- **Køb af ejendom**: Når en spiller lander på et ubebygget felt, kan de vælge at købe ejendommen.
- **Leje**: Hvis en spiller lander på en ejendom, som tilhører en anden spiller, skal de betale leje.
- **Chancekort**: Spillere, der lander på et "Chance"-felt, skal trække et kort, som enten kan give en belønning eller pålægge en straf.
- **Bygning af huse/hoteller**: Spillere kan opgradere deres ejendomme for at øge lejen.

## Projektstruktur

Projektet er opdelt i flere klasser for at adskille funktionalitet og gøre koden mere vedligeholdelsesvenlig:

- `Main.java` - Hovedindgangen til spillet.
- `Spiller.java` - Håndterer spillernes information og handlinger.
- `Ejendom.java` - Indeholder ejendommens detaljer og købsmekanismer.
- `Bræt.java` - Repræsenterer spillets bræt og felter.
- `Chancekort.java` - Indeholder logikken for håndtering af chancekort.

## Bidrag

Vi modtager gerne bidrag! Hvis du har idéer eller forbedringsforslag, kan du enten oprette en pull request eller åbne en issue.

