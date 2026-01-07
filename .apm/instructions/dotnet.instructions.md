---
applyTo: "**/*.cs"
---

# .NET Code Review Rules

## Architecture
- Respecter SOLID
- Pas de logique métier dans les Controllers
- Services injectés via DI

## Asynchronisme
- `async/await` obligatoire
- Interdiction de `.Result` et `.Wait()`

## Logging
- Logging structuré
- Pas d’interpolation dans les messages de log

## Exceptions
- Pas de catch vide
- Pas de `throw ex;` → utiliser `throw;`

## Tests
- Tests unitaires obligatoires pour la logique métier
- xUnit recommandé
