# Traceability Matrix — Contact Center Process Optimization

## Cel dokumentu

Macierz śladowania pokazuje powiązanie między problemami biznesowymi, wymaganiami, User Stories, procesem BPMN, modelem danych oraz KPI.

Celem macierzy jest pokazanie, że każdy element rozwiązania wynika z konkretnego problemu biznesowego i wspiera mierzalne cele operacyjne Contact Center.

---

## Traceability Matrix

| Problem biznesowy | Wymaganie biznesowe | Wymaganie funkcjonalne | User Story | Artefakt / proces | KPI |
|---|---|---|---|---|---|
| PB-01 Długi czas oczekiwania klientów na połączenie | BR-01 Skrócić czas oczekiwania w kolejce | FR-01 System powinien mierzyć czas oczekiwania klienta przed połączeniem z konsultantem | US-01 Jako lider Contact Center chcę monitorować czas oczekiwania, aby reagować na przeciążenie infolinii | BPMN AS-IS, BPMN TO-BE, SQL `calls` | ASA |
| PB-02 Wysoki poziom porzuconych połączeń | BR-02 Zmniejszyć liczbę porzuconych połączeń | FR-02 System powinien rejestrować porzucone połączenia i moment zakończenia oczekiwania | US-02 Jako lider Contact Center chcę analizować porzucone połączenia, aby usprawnić obsadę i kolejki | BPMN AS-IS, SQL `calls`, Power BI dashboard | Abandonment Rate |
| PB-03 Brak callbacku jako alternatywy dla kolejki | BR-03 Udostępnić klientowi możliwość wyboru oddzwonienia | FR-03 System powinien umożliwiać utworzenie żądania callbacku | US-03 Jako klient chcę wybrać callback, aby nie czekać w kolejce | BPMN TO-BE, API `POST /api/v1/callbacks`, SQL `callbacks` | Callback Rate, Callback Realization Rate |
| PB-04 Ograniczony zakres self-service w IVR | BR-04 Zwiększyć udział spraw obsłużonych automatycznie | FR-04 System powinien rozpoznawać sprawy możliwe do obsługi w IVR | US-04 Jako klient chcę załatwić prostą sprawę w IVR, aby nie czekać na konsultanta | BPMN TO-BE, SQL `calls` | Self-service Rate |
| PB-05 Niski poziom FCR | BR-05 Zwiększyć liczbę spraw rozwiązanych przy pierwszym kontakcie | FR-05 System powinien oznaczać, czy sprawa została rozwiązana przy pierwszym kontakcie | US-05 Jako lider zespołu chcę widzieć poziom FCR, aby identyfikować obszary wymagające poprawy | SQL `contacts`, SQL `cases`, Power BI dashboard | FCR |
| PB-06 Brak pełnej kontroli SLA | BR-06 Monitorować realizację spraw względem SLA | FR-06 System powinien rejestrować zdarzenia SLA i status przekroczenia terminu | US-06 Jako menedżer chcę monitorować SLA, aby priorytetyzować zaległe sprawy | SQL `sla_events`, Power BI dashboard | SLA Rate |
| PB-07 Brak analizy przyczyn kontaktu | BR-07 Umożliwić tagowanie powodu kontaktu i wyniku rozmowy | FR-07 System powinien zapisywać powód kontaktu oraz wynik rozmowy | US-07 Jako analityk chcę analizować powody kontaktu, aby wskazywać obszary do automatyzacji | BPMN TO-BE, SQL `contacts`, Power BI dashboard | Contact Reason Distribution |
| PB-08 Trudna identyfikacja spraw wymagających eskalacji | BR-08 Uporządkować obsługę eskalacji do 2nd line | FR-08 System powinien rejestrować eskalacje i status obsługi sprawy | US-08 Jako lider Contact Center chcę widzieć eskalacje, aby analizować przyczyny przekazywania spraw | BPMN AS-IS, BPMN TO-BE, SQL `cases` | Escalation Rate |
| PB-09 Brak spójnego modelu danych do raportowania | BR-09 Zapewnić model danych wspierający KPI Contact Center | FR-09 System powinien przechowywać dane o połączeniach, sprawach, kontaktach, konsultantach i klientach | US-09 Jako analityk BI chcę mieć spójny model danych, aby budować raporty KPI | SQL schema, sample data, KPI queries | Wszystkie KPI |
| PB-10 Ograniczona widoczność efektywności konsultantów | BR-10 Umożliwić analizę KPI na poziomie konsultanta i zespołu | FR-10 System powinien umożliwiać przypisanie kontaktu do konsultanta | US-10 Jako lider zespołu chcę analizować KPI konsultantów, aby wspierać coaching i planowanie obsady | SQL `agents`, SQL `contacts`, Power BI dashboard | AHT, FCR, SLA Rate |

---

## Podsumowanie

Macierz pokazuje, że projekt nie ogranicza się do samego modelu BPMN ani dashboardu. Każdy element rozwiązania jest powiązany z problemem biznesowym, wymaganiem, User Story, artefaktem projektowym oraz KPI.

Dzięki temu projekt pokazuje pełny sposób pracy analitycznej:

```text
Problem biznesowy → wymaganie → User Story → proces → dane → KPI → decyzja biznesowa
```
