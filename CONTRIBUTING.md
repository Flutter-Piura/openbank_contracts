# Contribuir a OpenBank Contracts

1. Revisa el plan maestro y ADR vigentes.
2. Describe el caso de uso antes de cambiar el contrato.
3. Añade ejemplos deterministas y exclusivamente ficticios.
4. Crea una rama corta desde `main` y usa Conventional Commits.

Ejemplos:

```text
feat(accounts): define account summary schema
fix(errors): require correlation identifier
docs(transfers): clarify idempotency header
```

Un PR debe indicar compatibilidad, consumidores afectados y estrategia de migración. Los importes usan unidades menores enteras con moneda explícita; las fechas usan ISO 8601 UTC y los IDs son opacos.

Los comandos de lint, bundle y breaking-change check se añadirán junto con OpenAPI. Hasta entonces ejecuta el workflow de higiene y `git diff --check`.

Al participar aceptas el [Código de conducta](CODE_OF_CONDUCT.md).
