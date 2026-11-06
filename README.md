# rimfrost-identitet-uppdaterad-asyncapi

AsyncAPI-spec som definierar det event som publiceras när identitetsdata har uppdaterats av en extern källa.

## Syfte

När identitetsdata uppdateras av en extern källa publiceras ett `IdentitetUppdateradEvent` till det topic som angavs vid registrering. Prenumeration och avregistrering hanteras via REST — se OpenAPI-specen för `rimfrost-service-identitet-prenumeration-openapi`.

## Event

| Kafka-topic | Riktning | Beskrivning |
|---|---|---|
| `replyTo` (angiven vid registrering) | ← service | `IdentitetUppdateradEvent` |

## Spec

Se [`asyncapi.yaml`](asyncapi.yaml) för fullständig meddelandedefinition.
