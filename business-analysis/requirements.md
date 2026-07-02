# Inżynieria wymagań

## Kontekst biznesowy

Proces Contact Center obejmuje obsługę połączeń przychodzących dotyczących faktur, reklamacji, spraw technicznych oraz zgłoszeń wymagających eskalacji do 2nd line lub back-office.

Analiza procesu AS-IS wykazała problemy wpływające na jakość obsługi klienta oraz efektywność operacyjną zespołu Contact Center.

---

## Zidentyfikowane problemy biznesowe

### PB-01

Wysoki poziom porzuconych połączeń w godzinach największego obciążenia.

### PB-02

Długi średni czas oczekiwania klienta na połączenie z konsultantem.

### PB-03

Ograniczony zakres samoobsługi w IVR dla prostych spraw.

### PB-04

Brak spójnego tagowania przyczyn kontaktu klienta.

### PB-05

Ograniczona możliwość bieżącego monitorowania SLA, FCR, AHT i callbacków.

---

## Wymagania biznesowe

### WB-01

Zmniejszenie liczby porzuconych połączeń.

### WB-02

Skrócenie średniego czasu oczekiwania klienta.

### WB-03

Zwiększenie udziału spraw obsługiwanych przez self-service.

### WB-04

Poprawa jakości danych o przyczynach kontaktu.

### WB-05

Zapewnienie monitorowania KPI operacyjnych w dashboardzie Power BI.

---

## Wymagania funkcjonalne

### WF-01

System powinien rejestrować każde połączenie przychodzące.

### WF-02

System powinien umożliwiać identyfikację klienta na podstawie danych z IVR lub CRM.

### WF-03

System powinien umożliwiać zapis przyczyny kontaktu klienta.

### WF-04

System powinien umożliwiać obsługę callbacku.

### WF-05

System powinien umożliwiać zapis statusu callbacku.

### WF-06

System powinien rejestrować informację o eskalacji sprawy do 2nd line.

### WF-07

System powinien udostępniać dane do raportowania KPI.

### WF-08

System powinien umożliwiać analizę SLA, FCR, AHT, ASA i porzuceń połączeń.

---

## Wymagania niefunkcjonalne

### WN-01

Czas odpowiedzi systemu dla podstawowych operacji nie powinien przekraczać 2 sekund.

### WN-02

Dostępność systemu powinna wynosić minimum 99,5%.

### WN-03

Wszystkie operacje użytkowników powinny być logowane.

### WN-04

Komunikacja między komponentami powinna być szyfrowana.

### WN-05

Rozwiązanie powinno umożliwiać obsługę minimum 10 000 połączeń dziennie.

---

## Źródła wymagań

Wymagania zostały zidentyfikowane na podstawie:

- analizy procesu AS-IS,
- analizy problemów operacyjnych,
- analizy KPI,
- mapowania przepływu danych,
- identyfikacji potrzeb interesariuszy,
- projektowania procesu TO-BE.
EOF
