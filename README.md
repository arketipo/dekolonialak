# Dekolonialak

Sistema para crear contenido conectando perfiles de diversidad.

## Descripción

Dekolonialak es una plataforma que facilita la creación de narrativas y contenido analizando y contrastando perspectivas desde diferentes perfiles de diversidad. El sistema ayuda a desmontar narrativas hegemónicas y construir versiones más plurales y contextualizadas.

## Stack

- **Frontend/App**: Lovable (React + Tailwind CSS)
- **Backend**: Supabase (PostgreSQL + Auth + Storage)
- **AI**: Claude API (análisis y generación de contenido)
- **Exportación**: Google Drive API (para equipo de comunicación)

## Fases

- **FASE 1 - MVP (3-4 días)**: Login, crear/abrir proyecto, subir documentación, contrastar, reconstruir, guardar y descargar
- **FASE 2 - Desarrollo**: RAG, análisis test dekolonialak, debatir, deconstruir, versiones
- **FASE 3 - Nice to have**: Colaboración avanzada, múltiples perspectivas, integraciones futuras

## Repositorio en Lovable

El código principal está en construcción en Lovable: https://dekolonialak.lovable.app/

Este repositorio actúa como respaldo y documentación del proyecto.

## Setup Local

```bash
git clone https://github.com/arketipo/dekolonialak.git
cd dekolonialak

# Configura variables de entorno
cp .env.example .env
# Edita .env con tus credenciales

# Instala dependencias (si trabajas localmente con código exportado)
npm install
```

## Variables de Entorno

Ver `.env.example` para todas las variables necesarias:
- Supabase credentials
- Claude API key
- Google Drive credentials

## Documentación

- `docs/ARQUITECTURA.md` - Decisiones técnicas y estructura
- `docs/FASES.md` - Detalles de cada fase
- `docs/LOVABLE.md` - Sincronización entre Lovable y este repo
