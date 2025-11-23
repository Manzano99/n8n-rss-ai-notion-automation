# 🤖 Smart RSS Aggregator with AI & Notion

Este proyecto es una automatización ETL (Extract, Transform, Load) construida en **n8n** que monitoriza múltiples fuentes de noticias tecnológicas, las resume usando IA y las archiva automáticamente en una base de datos de Notion.

## 🚀 Funcionalidades

- **Multi-Source Ingestion:** Monitoriza 5 feeds RSS diferentes (Dev.to, stackoverflow, etc.) diariamente.
- **AI Processing:** Utiliza **Google Gemini 2.0 Flash** para generar resúmenes en español y extraer palabras clave técnicas.
- **Deduplicación:** Lógica para seleccionar solo las noticias más relevantes de cada fuente.
- **Data Transformation:** Nodo de código (JavaScript) para limpieza de JSON y normalización de datos.
- **Notion Integration:** Carga automática con propiedades (Selects, URLs, Texto).

## 🛠️ Stack

- **n8n** (Workflow Automation)
- **Google Gemini API** (LLM para procesamiento de texto)
- **Notion API** (Base de datos / Frontend)
- **JavaScript** (Lógica de transformación de datos)

## 📋 Prerrequisitos para usar este workflow

Si quieres importar este flujo en tu instancia de n8n, necesitarás:

1.  **n8n** (Versión self-hosted o Cloud).
2.  **API Key de Google AI Studio** (Gemini).
3.  **Integración de Notion** configurada con acceso a una base de datos.
4.  Una base de datos en Notion con las columnas: `Título`, `URL`, `Resumen`, `KeyWords`, `Fuente`.

## 📸 Diagrama del Flujo

<img width="1013" height="527" alt="image" src="https://github.com/user-attachments/assets/8bcbc567-fe17-43fa-85bd-ce3f42e3b395" />
