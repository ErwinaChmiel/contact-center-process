# Podejście analityczne i struktura projektu

## Cel dokumentu

Dokument opisuje sposób przygotowania projektu Contact Center oraz uzasadnia podział repozytorium na foldery:

- `business-analysis/`
- `architecture/`
- `bpmn/`
- `sql/`
- `powerbi/`
- `docs/`

Celem takiej struktury było pokazanie pełnego procesu analitycznego: od identyfikacji problemu biznesowego, przez wymagania i proces TO-BE, aż po model danych, integracje, API oraz dashboard KPI.

Projekt nie został potraktowany wyłącznie jako raport Power BI ani sam diagram BPMN. Został uporządkowany jako case study pokazujące pracę na styku biznesu, procesów, danych i systemów.

---

## Logika pracy analitycznej

Dokumentacja została przygotowana zgodnie z następującą logiką:

```text
Problem biznesowy
        ↓
Interesariusze i potrzeby
        ↓
Wymagania biznesowe
        ↓
Wymagania funkcjonalne i niefunkcjonalne
        ↓
User Stories i kryteria akceptacji
        ↓
Backlog produktu
        ↓
Proces AS-IS i TO-BE w BPMN
        ↓
Architektura logiczna
        ↓
Integracje i REST API
        ↓
Model danych SQL
        ↓
Dashboard Power BI
        ↓
KPI i wnioski biznesowe
