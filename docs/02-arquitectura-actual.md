# 02 · Arquitectura actual (AS-IS)

## Producción real
```text
Usuarios / Google
      |
      v
tuformacionimporta.com
      |
  WordPress
   |     \
   |      -> Blog / contenido SEO
   v
 Airtable
   |
   v
Procesos manuales
```

## WeWeb
`tuformacionimporta.es` se usa como acceso interno al desarrollo. Inventario verificado el 30/09/2026:
- 32 páginas.
- 8 componentes no-code.
- 37 variables globales.

Incluye catálogo/buscador, landings, detalle de curso, acceso/registro, perfil, solicitudes y administración.

## Xano
Está apagado. No será runtime objetivo, pero debe auditarse antes de diseñar Supabase.

## Modelo relacional previo
Existe documentación histórica preparada para desarrolladores y debe compararse con Xano, Airtable, WeWeb y la visión futura.

## Riesgo principal
La funcionalidad actual está repartida entre software y conocimiento operativo humano. La migración debe capturar también las reglas manuales.
