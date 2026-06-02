---
layout: default
title: Pelipolku – Opiskelijatutorin ohjesivu
---

# Pelipolku: Opiskelijatutorin ohjesivu

Tämä sivu kokoaa Gradian opiskelijatutorille yhteen paikkaan keskeiset ohjeet, opintolinkit ja toimintamallit, kun tutorointi liittyy pelialan ristiinopiskeluun (Gradia x JAMK, tarvittaessa JYU-yhteistyö).

## Kenelle sivu on tarkoitettu?

- Gradian TVT-alan opiskelijalle, joka toimii tutorina pelipolulla
- Opiskelijalle, joka auttaa muita suunnittelemaan opintojen etenemistä pelialalle

## Mitä tutor tekee käytännössä?

- Auttaa opiskelijaa hahmottamaan opintopolun Gradia -> JAMK -> työelämä
- Ohjaa opiskelijaa oikeisiin opintojaksoihin ja hakemaan lisätietoa ajoissa
- Tukee projektityöskentelyssä (esim. game jamit, InnoFlash, TiCorporate)
- Kannustaa portfolion rakentamiseen ja verkostoitumiseen

```mermaid
flowchart TB

    ST(("🧑‍🎓 Opiskelijatutor"))

    G["Gradia tvt ohjelmistokehitys"]
    J["JAMK pelituotanto"]
    U["JYU tukevat opinnot"]

    L["Oppiminen \n ohjelmointi ja pelisuunnittelu"]
    C["Tekeminen \n projektit ja game jamit"]
    S["Näyttö \n demonurkkaus ja portfolio"]
    N["Verkostoituminen \n tapahtumata ja mentorit"]

    I["Peliala yritykset ja ammattilaiset"]

    ST --- G
    ST --- J
    ST --- U

    ST --- L
    ST --- C
    ST --- S
    ST --- N

    I --- L
    I --- C
    I --- S
    I --- N

        classDef student fill:#FFD54F,stroke:#333333,stroke-width:4px,color:#000000;

        classDef gradia fill:#2E7D32,color:#FFFFFF,stroke:#1B5E20,stroke-width:2px;
        classDef jamk fill:#500257,color:#FFFFFF,stroke:#0D004C,stroke-width:2px;
        classDef jyu fill:#5BBAD5,color:#FFFFFF,stroke:#2C8CA8,stroke-width:2px;

        classDef activity fill:#F3F4F6,color:#111827,stroke:#6B7280,stroke-width:2px;

        classDef industry fill:#FF8C42,color:#FFFFFF,stroke:#CC6E2B,stroke-width:3px;

    class ST student;
    class G gradia;
    class J jamk;
    class U jyu;

    class L,C,S,N activity;
    class I industry;
```

## Opintolinkit yhteen paikkaan

### JAMK tutkinto ja kurssit

- JAMK tutkinto: [Game Production -tutkinto-ohjelma](https://opetussuunnitelmat.peppi.jamk.fi/48/en/59/21547/1400)
- [Basic Programming](https://opetussuunnitelmat.peppi.jamk.fi/course/HG00CI46)
- [Game Programming](https://opetussuunnitelmat.peppi.jamk.fi/course/HG00CI44)
- [Game Engine](https://opetussuunnitelmat.peppi.jamk.fi/course/HG00CI47)

### Gradia tutkinto ja opintojaksot

- [Tieto- ja viestintätekniikan perustutkinto](https://eperusteet.opintopolku.fi/#/fi/ammatillinen/6779583/tutkinnonosat)
- [Ohjelmointi](https://eperusteet.opintopolku.fi/#/fi/ammatillinen/6779583/tutkinnonosat/6810819)
- [Ohjelmistokehittäjänä toimiminen](https://eperusteet.opintopolku.fi/#/fi/ammatillinen/6779583/tutkinnonosat/6810820)

## Tutorin toimintamalli opiskelijan tukemiseksi

```mermaid
flowchart LR

    A["🧑‍🎓 Opiskelijatutor"]

    B["Oppiminen kursseilla"]
    C["Tekeminen projektien avulla"]
    D["Osaamisen näyttäminen portfoliolla"]
    E["Verkostoituminen alan tapahtumissa"]

    A --> B
    A --> C
    A --> D
    A --> E

    B --> G["Gradia"]
    B --> J["JAMK"]
    B --> U["JYU"]

    C --> GP["Peliprojektit"]
    C --> GJ["Game jamit"]
    C --> TC["Ticorporate"]

    D --> DM["Demonurkkaus"]
    D --> PO["Portfolio"]

    E --> EV["Tapahtumat"]
    E --> ME["Mentorit"]
    E --> CO["Yritykset"]

    classDef student fill:#FFD54F,stroke:#333333,stroke-width:4px,color:#000000;

    classDef gradia fill:#2E7D32,color:white;
    classDef jamk fill:#500257,color:white;
    classDef jyu fill:#5BBAD5,color:white;

    classDef project fill:#E8F5E9, color:black;
    classDef showcase fill:#FFF3E0, color:black;
    classDef industry fill:#FF8C42,color:black;

    class A student;
    class G gradia;
    class J jamk;
    class U jyu;
    class D showcase;

    class GP,GJ,TC project;
    class DM,PO showcase;
    class EV,ME,CO industry;
```

## Etenemisen suositusaikajana

```mermaid
flowchart LR

    G1["Gradia ohjelmointi"]
    G2["Gradia ohjelmistokehittäjänä toimiminen"]

    BP["Basic Programming"]
    GE["Game Engine"]
    GP["Game Programming"]

    P["Projektit ja game jamit"]

    D["demonurkkaus"]

    I["yritykset peliala"]

    G1 --> BP
    G2 --> BP

    BP --> GE
    GE --> GP

    BP --> P
    GE --> P
    GP --> P

    P --> D

    D --> I

    I -.palaute.-> BP
    I -.mentorointi.-> GE
    I -.yhteistyö.-> GP

    classDef gradia fill:#2E7D32,color:white;
    classDef jamk fill:#500257,color:white;
    classDef industry fill:#FF8C42,color:white;
    classDef showcase fill:#5BBAD5,color:white;

    class G1,G2 gradia;
    class BP,GE,GP jamk;
    class D showcase;
    class I industry;
```

## Käytännön muistilista tutorille

- Varmista, että opiskelija löytää oikeat kurssikuvaukset linkeistä
- Tarkista, mitä osaamista opiskelija on jo hankkinut (hyväksiluku)
- Ohjaa opiskelija mukaan tapahtumiin: game jam, hackathon, InnoFlash, TiCorporate
- Suunnittele portfolioon 2-3 projektia
- Sopikaa seurantapiste 1-2 kuukauden päähän

## Usein kysytyt kysymykset

### 1) Pitääkö osata ohjelmoida etukäteen?

Ei välttämättä. Polku alkaa perusteista, mutta oma harjoittelu nopeuttaa etenemistä.

### 2) Missä järjestyksessä kurssit kannattaa tehdä?

Aloita Basic Programming -kurssilla, jatka Game Engine- ja Game Programming -kursseihin.

### 3) Miten tutor tukee eniten?

Selkein tuki tulee siitä, että tutor auttaa polusta kiinnostuneita, tekee yhteistyösä muiden tutorien kanssa.

## Yhteenveto

Opiskelijatutorin tehtävä on tehdä pelipolku näkyväksi ja käytännönläheiseksi: oikeat kurssit, oikea-aikainen tuki, aidot projektit ja jatkuva palautesykli. Tämä sivu toimii keskitettynä pikaoppaana arjen tutorointiin, ja sitä päivitetään tarpeen mukaan.