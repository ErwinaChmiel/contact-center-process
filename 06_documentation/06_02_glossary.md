# Glossary — Contact Center Process Optimization

## Cel dokumentu

Ten słownik zawiera najważniejsze pojęcia używane w projekcie optymalizacji procesu obsługi połączeń przychodzących w Contact Center.

Celem słownika jest ujednolicenie terminologii biznesowej, procesowej, systemowej i raportowej stosowanej w dokumentacji, modelach BPMN, SQL oraz dashboardzie Power BI.

---

## Słownik pojęć

| Termin | Definicja |
|---|---|
| Contact Center | Jednostka organizacyjna odpowiedzialna za obsługę kontaktów klientów, w tym połączeń telefonicznych, callbacków, spraw i eskalacji. |
| Klient | Osoba kontaktująca się z Contact Center w celu rozwiązania sprawy, uzyskania informacji lub zgłoszenia problemu. |
| Połączenie przychodzące | Kontakt telefoniczny zainicjowany przez klienta i obsługiwany przez system IVR lub konsultanta. |
| IVR | Interactive Voice Response — automatyczny system głosowy umożliwiający klientowi wybór tematu sprawy lub skorzystanie z samoobsługi. |
| Self-service | Automatyczna obsługa prostej sprawy przez klienta bez udziału konsultanta, np. w systemie IVR. |
| Callback | Oddzwonienie do klienta w późniejszym czasie, wybrane jako alternatywa dla oczekiwania w kolejce. |
| Kolejka | Etap procesu, w którym klient oczekuje na połączenie z konsultantem. |
| Konsultant 1st line | Konsultant pierwszej linii obsługi, odpowiedzialny za bezpośrednią obsługę większości spraw klientów. |
| 2nd line | Druga linia wsparcia, obsługująca sprawy trudniejsze, wymagające dodatkowej analizy lub specjalistycznej wiedzy. |
| Back Office | Zespół wspierający obsługę spraw wymagających analizy poza bezpośrednią rozmową z klientem. |
| Eskalacja | Przekazanie sprawy z 1st line do 2nd line lub back-office, gdy sprawa nie może zostać rozwiązana przy pierwszym kontakcie. |
| Sprawa | Zgłoszenie klienta dotyczące określonego problemu, pytania lub potrzeby obsługowej. |
| Kontakt | Pojedyncza interakcja klienta z Contact Center, np. rozmowa telefoniczna, callback lub kontakt w ramach sprawy. |
| Powód kontaktu | Kategoria opisująca, dlaczego klient skontaktował się z Contact Center, np. faktura, reklamacja, problem techniczny lub pytanie ogólne. |
| Wynik kontaktu | Rezultat kontaktu z klientem, np. rozwiązano, eskalowano, porzucono, callback zaplanowany. |
| Tagowanie kontaktu | Oznaczenie kontaktu odpowiednimi kategoriami, np. powodem kontaktu i wynikiem rozmowy, na potrzeby analizy KPI. |
| SLA | Service Level Agreement — ustalony poziom obsługi, np. maksymalny czas obsługi sprawy lub wymagany czas reakcji. |
| Zdarzenie SLA | Informacja o tym, czy dana sprawa została obsłużona w wymaganym czasie, czy przekroczyła SLA. |
| CRM | System zarządzania relacjami z klientami, przechowujący dane klienta, historię kontaktów i sprawy. |
| REST API | Interfejs wymiany danych między systemami, np. CRM, Contact Center, systemem callbacków i warstwą raportową. |
| OpenAPI | Standard opisu API w formacie czytelnym dla ludzi i narzędzi, umożliwiający dokumentowanie endpointów, parametrów, requestów i response’ów. |
| SQL Database | Relacyjna baza danych przechowująca dane potrzebne do analizy procesu Contact Center i wyliczania KPI. |
| Model danych | Struktura tabel i relacji opisująca sposób przechowywania danych o połączeniach, sprawach, kontaktach, klientach, konsultantach, callbackach i SLA. |
| Dane przykładowe | Zestaw testowych danych odzwierciedlających przykładowe scenariusze biznesowe, takie jak self-service, FCR, eskalacja, callback lub przekroczenie SLA. |
| KPI | Key Performance Indicator — kluczowy wskaźnik efektywności procesu. |
| Dashboard | Raport wizualny prezentujący KPI i wnioski operacyjne, przygotowany w Power BI. |
| Power BI | Narzędzie Business Intelligence służące do tworzenia raportów, dashboardów i analiz danych. |

---

## Słownik KPI

| KPI | Pełna nazwa | Definicja |
|---|---|---|
| ASA | Average Speed of Answer | Średni czas oczekiwania klienta na połączenie z konsultantem. |
| AHT | Average Handle Time | Średni czas obsługi kontaktu przez konsultanta, obejmujący rozmowę i czynności po rozmowie. |
| FCR | First Contact Resolution | Odsetek spraw rozwiązanych podczas pierwszego kontaktu z klientem, bez potrzeby kolejnego kontaktu lub eskalacji. |
| SLA Rate | Service Level Agreement Rate | Odsetek spraw lub kontaktów obsłużonych w wymaganym czasie SLA. |
| Abandonment Rate | Abandonment Rate | Odsetek połączeń porzuconych przez klientów przed połączeniem z konsultantem. |
| Self-service Rate | Self-service Rate | Odsetek spraw obsłużonych automatycznie w IVR bez udziału konsultanta. |
| Callback Rate | Callback Rate | Odsetek klientów, którzy wybrali callback zamiast oczekiwania w kolejce. |
| Callback Realization Rate | Callback Realization Rate | Odsetek callbacków, które zostały skutecznie zrealizowane. |
| Escalation Rate | Escalation Rate | Odsetek spraw przekazanych z 1st line do 2nd line lub back-office. |
| Contact Reason Distribution | Contact Reason Distribution | Rozkład powodów kontaktu klientów, np. faktury, reklamacje, sprawy techniczne lub pytania ogólne. |

---

## Statusy i wyniki procesu

| Pojęcie | Definicja |
|---|---|
| Połączenie obsłużone | Połączenie, które zakończyło się rozmową z konsultantem lub skuteczną samoobsługą w IVR. |
| Połączenie porzucone | Połączenie zakończone przez klienta przed połączeniem z konsultantem. |
| Sprawa otwarta | Sprawa, która została zarejestrowana, ale nie została jeszcze rozwiązana. |
| Sprawa w toku | Sprawa, nad którą trwa obsługa. |
| Sprawa eskalowana | Sprawa przekazana do 2nd line lub back-office. |
| Sprawa rozwiązana | Sprawa zakończona pozytywnym wynikiem obsługi. |
| Sprawa zamknięta | Sprawa formalnie zakończona w systemie. |
| Callback utworzony | Callback został zarejestrowany w systemie. |
| Callback zaplanowany | Callback ma przypisany termin realizacji. |
| Callback zrealizowany | Próba oddzwonienia została wykonana i zakończona zgodnie z procesem. |
| Callback anulowany | Callback został anulowany lub nie wymaga dalszej realizacji. |

---

## Pojęcia używane w modelu danych

| Tabela / obiekt | Znaczenie |
|---|---|
| `calls` | Tabela przechowująca dane o połączeniach przychodzących, czasie oczekiwania, kanale, statusie i wyniku połączenia. |
| `cases` | Tabela przechowująca sprawy klientów oraz ich statusy. |
| `contacts` | Tabela przechowująca informacje o kontaktach klienta z Contact Center. |
| `agents` | Tabela przechowująca dane konsultantów. |
| `customers` | Tabela przechowująca dane klientów. |
| `callbacks` | Tabela przechowująca żądania callbacków oraz ich statusy. |
| `sla_events` | Tabela przechowująca informacje o SLA, przekroczeniach i terminach obsługi. |

---

## Pojęcia API

| Pojęcie | Definicja |
|---|---|
| Endpoint | Adres API służący do wykonania konkretnej operacji, np. utworzenia callbacku lub pobrania danych klienta. |
| Request | Żądanie wysyłane do API. |
| Response | Odpowiedź zwracana przez API. |
| Payload | Dane przesyłane w request lub response, najczęściej w formacie JSON. |
| Status code | Kod odpowiedzi HTTP informujący o wyniku operacji, np. `200`, `201`, `400`, `404`. |
| Authorization | Mechanizm kontroli dostępu do API. |
| Customer ID | Unikalny identyfikator klienta. |
| Ticket ID | Unikalny identyfikator sprawy lub zgłoszenia. |
| Callback ID | Unikalny identyfikator callbacku. |

---

## Uwagi

Słownik ma charakter pomocniczy i wspiera spójne rozumienie terminów używanych w projekcie.

Pojęcia mogą być rozwijane w kolejnych wersjach projektu wraz z rozbudową procesu, modelu danych, API lub dashboardu.
