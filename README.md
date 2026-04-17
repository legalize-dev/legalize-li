# Legalize — Liechtenstein

> **Frühphase** — Dieses Repository befindet sich in aktiver Entwicklung. Dateistruktur, Commit-Verlauf und Inhalte können sich erheblich ändern, einschliesslich vollständiger Neugenerierung. Bauen Sie keine Tools auf der aktuellen Struktur auf, ohne mit grundlegenden Änderungen zu rechnen.
>
> **Early stage** — This repository is under active development. File structure, commit history, and content may undergo significant changes, including full regeneration.

Konsolidiertes liechtensteinisches Landesrecht in Markdown, versioniert mit Git.

Jedes Gesetz ist eine Datei. Jede Reform ist ein Commit.

Teil des Projekts [Legalize](https://github.com/legalize-dev/legalize) · [legalize.dev](https://legalize.dev)

## Struktur

```
li/
  LGBl-1921-015.md           — Verfassung des Fürstentums Liechtenstein
  LGBl-1926-004.md           — Personen- und Gesellschaftsrecht (PGR)
  LGBl-1988-037.md           — Strafgesetzbuch (StGB)
  LGBl-2010-340.md           — Steuergesetz (SteG)
  ...
```

Die Dateien sind nach ihrer LGBl-Nummer benannt (`LGBl-{Jahr}-{Nummer}`). Der normative Rang (Verfassung, Gesetz, Verordnung, Staatsvertrag) steht im YAML-Frontmatter jeder Datei, nicht in der Verzeichnisstruktur.

## Quelle

Daten von [gesetze.li (Lilex)](https://www.gesetze.li/), der amtlichen Gesetzesdatenbank des Fürstentums Liechtenstein, betrieben vom Rechtsdienst der Regierung (RDR).

Seit 1. Januar 2013 ist gemäss Art. 8 des Kundmachungsgesetzes (LGBl 2012 Nr. 174) ausschliesslich die signierte elektronische Fassung des LGBl rechtsverbindlich.

## Format

Jede Datei enthält:

- **YAML-Frontmatter**: Metadaten (Titel, LGBl-Nr, LR-Nr, Datum, Status, Quell-URL)
- **Markdown-Inhalt**: konsolidierter Text mit hierarchischer Gliederung
- **Fussnoten**: Verweise auf ändernde Erlasse als Markdown-Footnotes mit Links zu den jeweiligen LGBl-Einträgen

Die Versionsgeschichte jedes Gesetzes wird vollständig in der Git-Commit-Historie abgebildet. Eine Reform = ein Commit, datiert auf den Tag des Inkrafttretens der jeweiligen Fassung.

## Lizenz

Die Gesetzestexte sind als amtliche Werke gemeinfrei. Die Strukturierung, Formatierung und das Repository selbst stehen unter der [MIT](LICENSE)-Lizenz.

---

Teil von [legalize.dev](https://legalize.dev) · [Pipeline-Quellcode](https://github.com/legalize-dev/legalize-pipeline)
