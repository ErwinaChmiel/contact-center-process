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
