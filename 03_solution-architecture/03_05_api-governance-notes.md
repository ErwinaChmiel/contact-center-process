# API Governance Notes — Contact Center

## Cel

Dokument uzupełnia specyfikację REST API o standardy enterprise: bezpieczeństwo, idempotencję, obserwowalność, błędy i zasady kontraktów.

---

## Standardy API

| Obszar | Standard |
|---|---|
| Autoryzacja | OAuth2 Client Credentials / JWT |
| Uprawnienia | Scope'y: `contact-center.read`, `contact-center.write` |
| Idempotencja | Nagłówek `Idempotency-Key` dla operacji `POST` |
| Traceability | Nagłówek `X-Correlation-Id` w każdym request |
| Błędy | Jednolity model `code`, `message`, `traceId` |
| Paginacja | `limit`, `offset` albo cursor dla historii kontaktów |
| Audyt | Zapis zmian statusów callbacków i spraw |
| Rate limiting | Limity per klient API / system źródłowy |

---

## Przykładowy model błędu

```json
{
  "code": "CALLBACK_ALREADY_EXISTS",
  "message": "Callback for this source call has already been registered.",
  "traceId": "cc-api-20250101-000123"
}
```

---

## Eventy biznesowe

W architekturze docelowej warto rozważyć publikację eventów:

| Event | Kiedy powstaje | Konsumenci |
|---|---|---|
| `CallRegistered` | Rejestracja połączenia | Reporting, CRM |
| `CallbackRequested` | Klient wybiera callback | Dialer, Reporting |
| `CallbackCompleted` | Callback zrealizowany | CRM, Reporting |
| `CaseCreated` | Utworzono sprawę | Case Management, Reporting |
| `CaseEscalated` | Sprawa przekazana do 2nd line | Back Office, SLA Monitoring |
| `SlaBreached` | Przekroczono SLA | Alerts, Power BI |

---

## Wartość dla projektu

Dodanie `openapi.yaml` i governance notes pokazuje, że projekt uwzględnia nie tylko dokumentację analityczną, ale również wymagania implementacyjne typowe dla środowiska korporacyjnego.
