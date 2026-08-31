# OpenBank Contracts

Fuente de verdad para los contratos públicos de OpenBank.

> Todos los ejemplos representan identidades, cuentas y dinero ficticios.

## Contenido

```text
openapi/
└── openapi.yaml   # contrato autocontenido para API, MobileLab y generación
redocly.yaml       # reglas de lint
package.json       # comandos reproducibles
```

El contrato se diseña primero, se valida en CI y alimentará los mocks de MobileLab y el cliente Dart. Los cambios incompatibles requieren versionado explícito y son detectados por oasdiff.

## Validación local

```bash
npm ci
npm run lint
npm run bundle
npm run generate:dart
```

El bundle autocontenido se escribe en `dist/openapi.yaml` y el cliente en `generated/dart`; ambos son artefactos reproducibles y no se confirman en Git.

Consulta el [plan maestro](https://github.com/Flutter-Piura/openbank_docs/blob/main/PLAN_MAESTRO.md) y [ADR-0001](https://github.com/Flutter-Piura/openbank_docs/blob/main/adr/0001-clean-architecture-contract-first.md).

## Contribuir

Lee [CONTRIBUTING.md](CONTRIBUTING.md) y [SECURITY.md](SECURITY.md).

## Licencia

[MIT](LICENSE).
