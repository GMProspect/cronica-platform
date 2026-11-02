<div align="center">
  <h1>🏛️ CRÓNICA Engineering Group</h1>
  <p><em>Plataforma de Ingeniería Forense, Arquitectura y Análisis con IA Multimodal</em></p>

  [![Next.js](https://img.shields.io/badge/Next.js-15-black.svg)]()
  [![Gemini](https://img.shields.io/badge/Google_Gemini-2.0_Pro-blue.svg)]()
  [![WordPress](https://img.shields.io/badge/CMS-WordPress_Headless-21759B.svg)]()
  [![GraphQL](https://img.shields.io/badge/API-GraphQL-E10098.svg)]()
</div>

---

## 🎯 El Problema

La ingeniería forense y el análisis estructural en Venezuela enfrentan dos obstáculos críticos:

1. **Conocimiento fragmentado**: Los informes, normativas (ACI 318, ASTM, COVENIN) y análisis de fallas están dispersos en archivos estáticos o documentos físicos sin acceso rápido.
2. **Ausencia de asistencia técnica en campo**: Un profesional fuera de la oficina no tiene acceso inmediato a un experto que le ayude a interpretar una patología estructural visible en un video o fotografía.

**CRÓNICA** fue construida para resolver ambos problemas con tecnología de frontera.

---

## 🏗️ Arquitectura General

```mermaid
graph TD
    subgraph "Frontend (Next.js 15 App Router)"
        PUBLIC["Diario Técnico (Pública)"]
        LAB["The Lab — IA Multimodal"]
        DASHBOARD["Dashboard Global Operativo"]
    end

    subgraph "Fuentes de Datos"
        WP["WordPress Headless (CMS)"]
        GEMINI["Google Gemini 2.0 Flash/Pro"]
        STREAMS["Feeds en Tiempo Real (Sismos, Tráfico)"]
    end

    PUBLIC -- "Apollo Client / GraphQL" --> WP
    LAB -- "SDK Oficial" --> GEMINI
    DASHBOARD -- "APIs Públicas" --> STREAMS
```

---

## ✨ Módulos Clave

### 🧪 The Lab — Laboratorio de IA Multimodal
El componente central de la plataforma. Un asistente de IA configurado con un system prompt especializado en ingeniería forense, arquitectura y normativas de construcción venezolanas e internacionales. Capacidades:
- **Análisis de Video Frame-a-Frame**: Sube un video de una edificación con daños aparentes y la IA analiza cada fotograma buscando patrones de falla (grietas, desplazamientos, eflorescencias).
- **Consulta de Normativas**: Interpreta en lenguaje natural artículos del ACI, ASTM, COVENIN e ISO.
- **Diagnóstico Estructural Preliminar**: Describe una patología y recibe un informe de causas probables y recomendaciones.

### 📰 Diario Técnico (Headless CMS)
- Alimentado por **WordPress con WPGraphQL**.
- Contenido editorial de ingeniería, análisis de casos y novedades del sector.
- Consultas optimizadas vía **Apollo Client** con caché inteligente.

### 🌍 Dashboard Global
- Visualización en tiempo real de datos operativos de múltiples sedes.
- Integración de feeds públicos de actividad sísmica y tráfico aéreo regional.

---

## 🛠️ Stack Tecnológico

| Capa | Tecnología |
|---|---|
| **Framework** | Next.js 15 (App Router + React Server Components) |
| **IA / ML** | Google Gemini 2.0 Flash y Pro (SDK oficial) |
| **Data Fetching** | Apollo Client (GraphQL) |
| **CMS** | WordPress Headless + plugin WPGraphQL |
| **Estilos** | Tailwind CSS |

---

> Proyecto privado desarrollado por **Gustavo Matheus** para CRÓNICA Engineering Group.
