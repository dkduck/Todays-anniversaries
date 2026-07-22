# 🎉 TODAY – Dynamisk Dagsinfo-kort til Home Assistant

Et rent, elegant og fuldautomatisk *"Hvilken dag er det i dag?"*-kort til Home Assistant, bygget med **custom:button-card** og ren JavaScript-logik.

Kortet viser et dagligt ikon, en titel og en undertekst — herunder helligdage, flagdage, FN-dage, uofficielle temadage og personlige begivenheder.

---

## ✨ Funktioner

- **Automatisk datogenkendelse**
- **100+ danske helligdage, temadage og kulturelle mærkedage**
- **Understøttelse af personlige begivenheder** (fødselsdage, mærkedage)
- **Flot layout** med ikon, overskrift og beskrivelse
- **Automatisk datoberegning** for variable mærkedage, hvor datoen ændrer sig hvert år
- **Fallback-besked** når der ikke findes en mærkedag
- **Transparent baggrund** og pixel-perfekt Home Assistant-styling
- **Ingen afhængigheder** udover `custom:button-card`

---

## 📦 Installation

### Krav

- Home Assistant
- HACS
- `custom:button-card` installeret

### Tilføjelse af kortet

1. Åbn dit Home Assistant-dashboard
2. Tilføj et **Manuelt kort**
3. Indsæt YAML'en fra filen `/card.yaml` i dette repository

Kortet finder automatisk dagens dato og viser den rette begivenhed.

---

## 🧠 Sådan fungerer det

Kortet bruger et JavaScript-opslagsobjekt, der indeholder alle mærkedage i formatet:

```js
"DD-MM": { ikon: "🎉", tekst: "Titel", sub: "Beskrivelse" }
```

Dagens dato genkendes automatisk, og den matchende entry vises.

Hvis der ikke findes en entry, vises en fallback-besked:

> *"Bare en helt almindelig dag"*

---

## 🛠️ Tilpasning

Du kan nemt:

- Tilføje nye mærkedage
- Ændre ikoner, titler eller beskrivelser
- Ændre farver, så de matcher dit dashboard-tema
- Erstatte fallback-teksten med din egen formulering

Al tilpasning sker inde i `dage`-objektet i YAML-filen.

---

## 🚀 Fremtidige idéer

- Sæsonbestemte farvetemaer
- API-baseret flagdagsgenkendelse
- Integration med kalender-sensor
- Animerede ikoner på mærkedage

---

## ❤️ Bidrag

Pull requests er velkomne — især nye mærkedage, styling-forbedringer eller optimeringer.

---

## 📜 Licens
