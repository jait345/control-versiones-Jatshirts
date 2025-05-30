# Proyecto: control-versiones-Jatshirts

Este repositorio implementa un flujo de trabajo basado en **Git Flow**, ideal para equipos que requieren control riguroso sobre versiones, desarrollo colaborativo y despliegue estructurado.

---

## 🛠️ Estructura del Flujo de Versionamiento

Se sigue el modelo **Git Flow**, con las siguientes ramas principales:

- `main`: código en producción (estable).
- `develop`: rama de integración para el desarrollo activo.
- `feature/*`: nuevas funcionalidades creadas desde `develop`.
- `release/*`: preparación de versiones estables, desde `develop`.
- `hotfix/*`: correcciones urgentes sobre `main`.

### Diagrama de Flujo

```plaintext
main ────●─────────────●───────────────●─────────────→
          ╲             ╲               ╲
           ╲ hotfix/*    ╲ hotfix/*      ╲
develop ──→●──────●──────●──────●──────→●────────────→
             ╲      ╲       ╲       ╲
          feature/* feature/*  release/*
