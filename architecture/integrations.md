# Analiza integracji

## Cel dokumentu

Celem dokumentu jest opisanie koncepcyjnej integracji pomiędzy komponentami rozwiązania Contact Center oraz określenie głównych przepływów danych wykorzystywanych w procesie obsługi połączeń i raportowania KPI.

---

## Komponenty rozwiązania

- IVR,
- system Contact Center,
- CRM,
- relacyjna baza danych SQL,
- Power BI.

---

## Przepływ danych

```text
IVR
  ↓
Contact Center
  ↓
CRM
  ↓
SQL Database
  ↓
Power BI

Integracja IVR z Contact Center
Cel
Przekazanie informacji o wyborach klienta w IVR do systemu Contact Center.
Dane

numer telefonu,
temat sprawy,
wybór self-service,
wybór callbacku,
czas rozpoczęcia połączenia.


Integracja Contact Center z CRM
Cel
Udostępnienie konsultantowi danych klienta i historii kontaktów.
Dane

identyfikator klienta,
segment klienta,
status klienta,
historia zgłoszeń,
aktywne sprawy.


Integracja z bazą SQL
Cel
Zasilenie modelu danych wykorzystywanego do analizy operacyjnej i raportowania KPI.
Dane

połączenia,
zgłoszenia,
kontakty,
konsultanci,
klienci,
callbacki,
SLA.


Integracja SQL z Power BI
Cel
Budowa dashboardu operacyjnego dla liderów i menedżerów Contact Center.
Dane raportowe

FCR,
SLA,
AHT,
ASA,
Abandonment Rate,
Callback Rate,
Self-service Rate.
EOF
