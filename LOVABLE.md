# Sincronización Lovable ↔ GitHub

## Estructura

El código principal se desarrolla en Lovable:
- **URL**: https://dekolonialak.lovable.app/
- **Ventaja**: Desarrollo rápido, preview en tiempo real
- **Stack interno**: React + Tailwind en Lovable

## Respaldo en GitHub

Este repositorio actúa como:
1. **Backup** de todo el código y documentación
2. **Control de versiones** desde Lovable
3. **Documentación histórica** del proyecto
4. **Referencia** para futuras iteraciones

## Flujo de Sincronización

### Exportar de Lovable
1. En Lovable, generar export de código (React + CSS)
2. Copiar a carpeta `src/` en este repo
3. Commit con mensaje: "Export Lovable - [feature/componente]"

### Código a Sincronizar
- Componentes React
- Estilos Tailwind
- Páginas/rutas
- Utilities y helpers
- .env (como template en .env.example)

### NO Sincronizar
- node_modules
- .env (archivo real, solo template)
- Build artifacts

## Cadencia

- **Diaria (final de sesión)**: Pequeños exports de features completadas
- **End of phase**: Full export y tageo de versión

## Tagging

Versiones siguiendo patrón:
- `v0.1.0-alpha` - MVP
- `v0.2.0-alpha` - Fase 2
- `v1.0.0` - Producción

## URLs de Referencia

- Código en desarrollo: https://dekolonialak.lovable.app/
- Repo backup: https://github.com/arketipo/dekolonialak
- Issues/tracking: GitHub Issues
