# Fases de Desarrollo Dekolonialak

## FASE 1 - MVP (3-4 días, ~16.5 horas)

Funcionalidad básica para validar el concepto y flujo principal.

### Features

- Autenticación usuario (login/signup)
- Crear nuevo proyecto
- Abrir proyecto existente
- Subir documentación (selector formato: texto/imagen/audio/video)
- Contrastar (chat conversacional con Claude)
- Reconstruir/crear narrativa (genera contenido nuevo)
- Guardar resultados en Supabase
- Descargar .zip con outputs

### Sección Cero
- Selector condicional de formato que carga dinámicamente solo tabs relevantes
- UX simplificada para MVP

### Arquitectura
- Supabase: users, projects, documents, narratives (básico)
- Claude API: chat + generación
- Google Drive: export (opcional MVP)

### Criterios de Aceptación
- Usuario puede completar flujo end-to-end
- Documentación guardada correctamente
- Chat funcional
- Descarga .zip con resultados

---

## FASE 2 - Desarrollo (semanas 2-4)

Expansión de capacidades analíticas y trazabilidad.

### Features

- RAG (Retrieval Augmented Generation) con histórico de proyectos
- Test Dekolonialak (5 dimensiones de análisis)
- Debatir (múltiples perspectivas en mismo documento)
- Deconstruir (análisis profundo de narrativas)
- Sistema de versiones con trazabilidad
- Colaboración básica (comentarios)
- Metadata enriquecida en narrativas

### BD Enhancements
- Tablas: debates, versions, comments
- Campos: version_parent_id, debate_round, analysis_dimensions

### AI Enhancements
- Prompts más sofisticados para cada operación
- RAG context window
- Análisis dimensional

---

## FASE 3 - Nice to Have (Futuro)

Features de madurez y escalabilidad.

### Features

- Archivo colectivo (dataset de narrativas)
- Perspectivas múltiples (perfiles de diversidad precargados)
- Colaboración avanzada (real-time, roles, permisos)
- Admin avanzado (users, billing, analytics)
- Múltiples proveedores IA (switcheable)
- UX optimizaciones (dark mode, mobile, a11y)
- Integraciones futuras (Slack, Discord, etc)
- Export a más formatos (PDF, HTML, Notion)

### BD Enhancements
- Organizaciones/workspaces
- Roles y permisos granulares
- Analytics tables

---

## Tracking

- Horas presupuestadas FASE 1: 16.5h
- Tracking en `horas proyecto dekolonialak.md` en Obsidian
- Decisiones guardadas en memoria
