# Specyfikacja REST API

## Cel dokumentu

Dokument opisuje przykładowe endpointy REST API dla rozwiązania Contact Center.  
Specyfikacja ma charakter analityczny i pokazuje sposób opisu integracji systemowych z perspektywy analityka biznesowo-systemowego.

---

## 1. Utworzenie callbacku

### Endpoint

POST /api/v1/callbacks

### Opis

Endpoint służy do utworzenia zgłoszenia callbacku dla klienta, który nie chce oczekiwać w kolejce.

### Request

```json
{
  "customerId": 1001,
  "phoneNumber": "+48123456789",
  "preferredTime": "2026-07-01T14:30:00",
  "reason": "invoice"
}
