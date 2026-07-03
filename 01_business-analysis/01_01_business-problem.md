# Analiza problemu biznesowego — Contact Center

## Cel dokumentu

Celem dokumentu jest opisanie problemów biznesowych zidentyfikowanych w procesie obsługi połączeń przychodzących w Contact Center oraz określenie ich wpływu na klienta, konsultantów, proces operacyjny i KPI.

Dokument stanowi punkt wyjścia do dalszej analizy wymagań, projektowania procesu TO-BE, backlogu produktu oraz dashboardu KPI.

---

## Kontekst biznesowy

Contact Center obsługuje połączenia przychodzące dotyczące m.in.:

- faktur,
- reklamacji,
- problemów technicznych,
- spraw wymagających eskalacji do 2nd line,
- spraw możliwych do obsługi przez self-service lub callback.

Analiza procesu AS-IS wykazała problemy wpływające na jakość obsługi klienta oraz efektywność operacyjną zespołu Contact Center.

---

## Zidentyfikowane problemy biznesowe

| ID | Problem biznesowy | Opis | Wpływ na organizację |
|---|---|---|---|
| PB.01 | Wysoki czas oczekiwania klienta | Klienci długo oczekują na połączenie z konsultantem w godzinach szczytu | Spadek satysfakcji klienta i wzrost liczby porzuconych połączeń |
| PB.02 | Wysoki poziom porzuconych połączeń | Część klientów rozłącza się przed uzyskaniem połączenia z konsultantem | Utracone kontakty, ryzyko ponownych zgłoszeń i niższa jakość obsługi |
| PB.03 | Ograniczona samoobsługa klienta | Proste sprawy wymagają kontaktu z konsultantem zamiast obsługi w IVR | Większe obciążenie konsultantów i wyższe koszty operacyjne |
| PB.04 | Niewystarczająca kontrola SLA | Brak pełnej widoczności spraw zagrożonych przekroczeniem terminu | Opóźniona reakcja liderów zespołu i ryzyko niedotrzymania SLA |
| PB.05 | Ograniczona analiza przyczyn kontaktu | Brak spójnego tagowania powodów kontaktu klienta | Trudność w identyfikacji głównych źródeł zgłoszeń i optymalizacji procesu |

---

## Wpływ biznesowy

| Obszar | Wpływ |
|---|---|
| Klient | Dłuższy czas oczekiwania, konieczność ponownego kontaktu, niższa satysfakcja |
| Konsultant | Większe obciążenie, obsługa powtarzalnych spraw, brak pełnego kontekstu klienta |
| Lider zespołu | Ograniczona widoczność KPI, trudniejsza identyfikacja problemów operacyjnych |
| Menedżer Contact Center | Trudność w podejmowaniu decyzji na podstawie danych |
| Organizacja | Wyższe koszty operacyjne i niższa efektywność procesu |

---

## Skutki operacyjne

| Problem | Skutek operacyjny |
|---|---|
| Długi czas oczekiwania | Większe kolejki i większe ryzyko porzucenia połączenia |
| Porzucone połączenia | Klient może kontaktować się ponownie, zwiększając wolumen zgłoszeń |
| Brak self-service | Konsultanci obsługują sprawy, które mogłyby być zautomatyzowane |
| Brak pełnego monitorowania SLA | Sprawy przekroczone po terminie są identyfikowane z opóźnieniem |
| Brak spójnego tagowania | Dashboard KPI nie pokazuje pełnego obrazu przyczyn kontaktu |

---

## Powiązane KPI

| KPI | Powiązany problem | Cel analizy |
|---|---|---|
| ASA | PB.01 | Pomiar średniego czasu oczekiwania na odpowiedź |
| Abandonment Rate | PB.02 | Monitorowanie odsetka porzuconych połączeń |
| Self-service Rate | PB.03 | Ocena udziału spraw obsłużonych automatycznie |
| SLA Rate | PB.04 | Monitorowanie terminowości obsługi |
| FCR Rate | PB.05 | Ocena skuteczności rozwiązania sprawy przy pierwszym kontakcie |
| AHT | PB.01, PB.03 | Analiza średniego czasu obsługi połączenia |
| Callback Realization Rate | PB.02 | Ocena skuteczności mechanizmu callback |

---

## Cele biznesowe procesu TO-BE

| ID | Cel biznesowy | Powiązany problem |
|---|---|---|
| CB.01 | Skrócenie średniego czasu oczekiwania klienta | PB.01 |
| CB.02 | Zmniejszenie liczby porzuconych połączeń | PB.02 |
| CB.03 | Zwiększenie wykorzystania self-service w IVR | PB.03 |
| CB.04 | Poprawa monitorowania SLA i alertów operacyjnych | PB.04 |
| CB.05 | Poprawa jakości danych o przyczynach kontaktu | PB.05 |
| CB.06 | Umożliwienie podejmowania decyzji operacyjnych na podstawie dashboardu KPI | PB.01 - PB.05 |

---

## Oczekiwana wartość biznesowa

| Obszar | Oczekiwana wartość |
|---|---|
| Obsługa klienta | Krótszy czas oczekiwania i szybsze rozwiązanie sprawy |
| Efektywność operacyjna | Lepsze wykorzystanie pracy konsultantów |
| Raportowanie | Większa widoczność KPI i wyjątków operacyjnych |
| Zarządzanie | Lepsze decyzje dotyczące grafików, kolejek i priorytetów |
| Jakość danych | Spójne dane do analizy powodów kontaktu i skuteczności obsługi |

---

## Założenia analityczne

| ID | Założenie |
|---|---|
| ZA.01 | Projekt bazuje na przykładowym procesie Contact Center |
| ZA.02 | Dane wykorzystane w projekcie są danymi przykładowymi |
| ZA.03 | Analiza koncentruje się na procesie, danych, KPI i raportowaniu |
| ZA.04 | Projekt nie obejmuje pełnej implementacji produkcyjnej systemu Contact Center |
| ZA.05 | Proces TO-BE uwzględnia self-service, callback, tagowanie i monitoring KPI |

---

## Podsumowanie

Analiza problemu biznesowego wskazuje, że główne obszary wymagające usprawnienia dotyczą czasu oczekiwania, liczby porzuconych połączeń, ograniczonej samoobsługi, kontroli SLA oraz jakości danych o przyczynach kontaktu.

Zidentyfikowane problemy zostały wykorzystane jako podstawa do:

- zaprojektowania procesu TO-BE,
- określenia wymagań biznesowych i funkcjonalnych,
- przygotowania backlogu produktu,
- zdefiniowania KPI,
- zaprojektowania modelu danych SQL,
- budowy dashboardu Power BI.

