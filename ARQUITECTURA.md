# Arquitectura Dekolonialak

## Decisiones Técnicas

### Frontend
- **Framework**: React (vía Lovable)
- **Styling**: Tailwind CSS
- **Hosting**: Lovable (https://dekolonialak.lovable.app/)
- **Reason**: Desarrollo rápido manteniendo control del código

### Backend
- **Base de datos**: Supabase (PostgreSQL)
- **Autenticación**: Supabase Auth
- **Storage**: Supabase Storage (documentos de entrada)
- **Reason**: Escalable, open source, integración sencilla con AI

### AI
- **Proveedor**: Anthropic (Claude API)
- **Casos de uso**:
  - Análisis de documentación (chat conversacional)
  - Generación de narrativas (reconstrucción/creación)
  - Test Dekolonialak (análisis en 5 dimensiones)
- **Reason**: Capacidad de análisis profundo y multimodal

### Exportación
- **Google Drive API**: Exportar resultados para equipo comunicación
- **Reason**: Facilita colaboración con equipo externo

## Estructura de Base de Datos

```
users
├── id (UUID)
├── email
├── name
└── created_at

projects
├── id (UUID)
├── user_id (FK)
├── name
├── description
└── created_at

documents
├── id (UUID)
├── project_id (FK)
├── title
├── content (texto/imagen/audio/video)
├── content_type (enum)
└── created_at

narratives
├── id (UUID)
├── document_id (FK)
├── type (comparison/version/analysis/debate)
├── content
├── metadata (json)
└── created_at
```

## Flujo Principal (MVP)

1. Usuario login → Supabase Auth
2. Crear/abrir proyecto
3. Subir documentación (multi-formato)
4. Contrastar con Claude API (análisis)
5. Reconstruir/crear narrativa (Claude API)
6. Guardar en Supabase
7. Descargar .zip con resultados

## Próximas Integraciones (Fase 2-3)

- RAG para histórico de proyectos
- Test Dekolonialak (5 dimensiones predefinidas)
- Colaboración en tiempo real
- Múltiples versiones con trazabilidad
