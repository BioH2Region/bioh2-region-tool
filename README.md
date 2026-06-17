# BioH2Region — Regulatorik-Wegweiser für KMU

> Interaktiver Wegweiser durch die regulatorischen Rahmenbedingungen der Wasserstoffwirtschaft in Bayern und Oberösterreich, zugeschnitten auf kleine und mittlere Unternehmen (KMU).

**🔗 Live-Tool:** [bioh2region.github.io/bioh2-region-tool](https://bioh2region.github.io/bioh2-region-tool/)

---

## Über das Tool

Dieses Tool führt KMU in fünf Schritten durch die relevanten regulatorischen, fördertechnischen und regionalen Informationen rund um die Wasserstoff-Wertschöpfungskette:

1. **Region** — Bayern oder Oberösterreich
2. **Vorhaben** — Elektrolyseur, Biomasse-Anlage, Brennstoffzelle, Wasserstoffspeicher oder geführte Einstiegsberatung
3. **Erste Schritte & Regulatorik** — EU-, nationale und regionale Vorschriften mit praktischer Bedeutung für KMU
4. **Vor Ort** — aktive Landkreise und Städte in der Kompetenzregion mit Potenzialanalyse und Best-Practice-Beispielen
5. **Kontakt** — direkter Draht zu den Projektpartnern für individuelle Beratung

Bei der Option *"Ich bin offen — kurze Beratung"* erfolgt eine kurze Bedarfsanalyse (drei Fragen zu Sektor, verfügbaren Ressourcen und Investitionsumfang), aus der eine konkrete Einstiegsempfehlung generiert wird.

## Projektkontext

Dieses Tool entstand im Rahmen des Projekts **BioH2Region** (Förderkennzeichen BA0100157), kofinanziert aus dem Programm **Interreg VI-A Bayern–Österreich 2021–2027** und der Europäischen Union.

Es ist Teil der Aktivität 2.1 *„Begriffsdefinitionen und Regulatorik"* mit dem Ziel, die teils komplexen rechtlichen Rahmenbedingungen für die Wasserstoffanwendung in KMU zugänglich aufzubereiten.

## Projektpartner

| Partner | Land | Website |
|---|---|---|
| Hochschule Landshut (Trägerhochschule) | DE | [haw-landshut.de](https://www.haw-landshut.de/) |
| Technologiezentrum Energie (TZE) | DE | [tze.haw-landshut.de](https://www.haw-landshut.de/forschung/forschungseinrichtungen/technologiezentrum-energie.html) |
| CenTouris | DE | [centouris.de](https://www.centouris.de/) |
| FH Oberösterreich, Campus Wels | AT | [fh-ooe.at](https://www.fh-ooe.at/) |
| Business Upper Austria | AT | [biz-up.at](https://www.biz-up.at/) |

## Technische Details

- **Single-File HTML** — keine externen Abhängigkeiten außer Google Fonts
- **Vollständig clientseitig** — funktioniert offline, sobald geladen
- **Eingebettete Logos** als Base64 für maximale Portabilität
- **Datenstruktur** als JavaScript-Arrays direkt in `index.html` — Regulierungen, Standorte und Kontakte sind leicht editierbar

## Lokal ausführen

```bash
git clone https://github.com/BioH2Region/bioh2-region-tool.git
cd bioh2-region-tool
# index.html im Browser öffnen — fertig
```

## Inhalte aktualisieren

Die drei zentralen Datenstrukturen befinden sich im `<script>`-Block von `index.html`:

| Datensatz | Suchmarker im Code |
|---|---|
| Regulierungen | `// REGULATION DATABASE` |
| Landkreise / Städte | `// KOMPETENZREGION DATA` |
| Projektpartner-Kontakte | `// CONTACT DATA` |

Änderungen werden per Git-Push automatisch auf die GitHub-Pages-URL übernommen.

## Rechtlicher Hinweis

Die in diesem Tool bereitgestellten Informationen dienen ausschließlich der allgemeinen Orientierung und stellen **keine Rechts-, Steuer- oder Förderberatung** dar. Für verbindliche Entscheidungen ist die individuelle Beratung durch qualifizierte Rechtsanwält:innen, Steuerberater:innen oder Energieberater:innen erforderlich. Die Projektpartner des BioH2Region-Konsortiums übernehmen keine Haftung für Aktualität, Vollständigkeit oder Richtigkeit der Inhalte. Maßgeblich sind ausschließlich die jeweils verlinkten Originalquellen in ihrer aktuell gültigen Fassung.

## Lizenz

MIT — siehe [LICENSE](./LICENSE).

Diese offene Lizenzierung erlaubt es Projektpartnern und Dritten, das Tool zu nutzen, anzupassen und weiterzuverbreiten, sofern die Urheberschaft anerkannt wird.

## Förderhinweis

![Kofinanziert von der Europäischen Union — Interreg Bayern-Österreich](https://bioh2region.eu/wp-content/uploads/2025/01/INTERREG_Logo_RGB_fuer_weisser_HG-1536x338.webp)

Dieses Tool wurde im Rahmen des Projekts *BioH2Region* (BA0100157) entwickelt, kofinanziert vom Programm Interreg VI-A Bayern–Österreich 2021–2027 und der Europäischen Union.

Mehr zum Projekt: [bioh2region.eu](https://bioh2region.eu/)
