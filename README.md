# Contact Center Process Optimization — BPMN + SQL + Power BI

> Portfolio project showing a full business, process, system, data and BI analysis case study for a Contact Center process.

https://img.shields.io/badge/Business%20Analysis-Requirements-blue
https://img.shields.io/badge/BPMN-AS--IS%20%7C%20TO--BE-green
https://img.shields.io/badge/SQL-Data%20Model-orange
https://img.shields.io/badge/API-OpenAPI%203.0-lightgrey
https://img.shields.io/badge/Power%20BI-KPI%20Dashboard-yellow
https://img.shields.io/badge/Portfolio-Business%20%7C%20BI%20Analyst-purple

---

## O projekcie

Projekt przedstawia kompletne case study optymalizacji procesu obsługi połączeń przychodzących w Contact Center.

Celem projektu jest pokazanie pełnego toku pracy analitycznej — od identyfikacji problemu biznesowego, przez analizę wymagań i modelowanie procesu BPMN AS-IS / TO-BE, aż po zaprojektowanie architektury logicznej, integracji, specyfikacji API, modelu danych SQL oraz dashboardu KPI w Power BI.

Projekt został przygotowany jako portfolio analityczki biznesowo-systemowej i BI, pokazujące pracę na styku:

- biznesu,
- procesów,
- systemów,
- danych,
- SQL,
- REST API,
- OpenAPI,
- raportowania KPI,
- Power BI.

---

## Cel projektu

Celem projektu jest zaprezentowanie, w jaki sposób można przejść od problemów operacyjnych w Contact Center do uporządkowanego rozwiązania analityczno-systemowego.

Projekt obejmuje:

- analizę problemu biznesowego,
- analizę interesariuszy,
- inżynierię wymagań,
- User Stories i kryteria akceptacji,
- backlog produktu,
- modelowanie procesu BPMN AS-IS i TO-BE,
- opis architektury logicznej rozwiązania,
- analizę integracji między systemami,
- przykładową specyfikację REST API,
- plik OpenAPI zgodny ze standardem OpenAPI 3.0,
- projekt relacyjnego modelu danych SQL,
- dane przykładowe,
- zapytania SQL dla KPI,
- dashboard operacyjny w Power BI,
- analizę KPI: FCR, SLA, AHT, ASA, Abandonment Rate, Callback Rate, Self-service Rate.

---

## Zakres biznesowy

Projekt dotyczy procesu obsługi połączeń przychodzących w Contact Center.

W analizie uwzględniono:

- obsługę połączeń przez IVR,
- klasyfikację tematu kontaktu,
- obsługę przez konsultanta 1st line,
- eskalację do 2nd line / back-office,
- samoobsługę w IVR,
- callback jako alternatywę dla oczekiwania w kolejce,
- monitorowanie SLA,
- oznaczanie przyczyny kontaktu i wyniku rozmowy,
- przygotowanie danych pod raportowanie KPI.

---

## Główne problemy biznesowe

W procesie AS-IS zidentyfikowano następujące problemy:

- długi czas oczekiwania klientów na połączenie,
- wysoki poziom porzuconych połączeń,
- ograniczony zakres samoobsługi w IVR,
- brak callbacku jako alternatywy dla oczekiwania w kolejce,
- niewystarczającą kontrolę SLA,
- ograniczoną analizę przyczyn kontaktu,
- brak pełnej widoczności KPI operacyjnych,
- utrudnione monitorowanie efektywności konsultantów,
- brak spójnego modelu danych do raportowania.

Proces TO-BE odpowiada na te problemy poprzez:

- self-service w IVR dla prostych spraw,
- callback dla klientów oczekujących w kolejce,
- tagowanie przyczyn kontaktu i wyniku rozmowy,
- lepsze monitorowanie SLA,
- sprawniejszą eskalację do 2nd line,
- przygotowanie danych do raportowania KPI,
- uporządkowany model danych SQL,
- dashboard Power BI dla liderów i menedżerów.

---

## Pytania biznesowe, na które odpowiada projekt

Dashboard i dokumentacja analityczna odpowiadają m.in. na pytania:

- W których godzinach Contact Center ma największe obciążenie?
- Jaki jest poziom FCR i SLA dla całego procesu oraz poszczególnych zespołów?
- Które typy spraw najczęściej wymagają eskalacji do 2nd line?
- Ilu klientów korzysta z self-service w IVR?
- Ilu klientów wybiera callback zamiast oczekiwania w kolejce?
- Czy callbacki są realizowane terminowo?
- Którzy konsultanci mają podwyższony AHT lub niższy FCR?
- Ile spraw przekroczyło SLA?
- Jakie kategorie kontaktu generują największe obciążenie?
- Jakie usprawnienia mogą zmniejszyć liczbę porzuconych połączeń?

---

## Logika projektu

Projekt został uporządkowany zgodnie z naturalną kolejnością pracy analitycznej:

```text
Problem biznesowy
        ↓
Interesariusze i potrzeby
        ↓
Wymagania biznesowe, funkcjonalne i niefunkcjonalne
        ↓
User Stories i kryteria akceptacji
        ↓
Backlog produktu
        ↓
Proces AS-IS i TO-BE w BPMN
        ↓
Architektura logiczna rozwiązania
        ↓
Integracje i REST API
        ↓
Specyfikacja OpenAPI
        ↓
Model danych SQL
        ↓
Dane przykładowe
        ↓
Zapytania KPI
        ↓
Dashboard Power BI
        ↓
Wnioski biznesowe i rekomendacje
