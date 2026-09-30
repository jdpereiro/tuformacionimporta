# 03 · Arquitectura objetivo provisional

```text
                        GitHub
                          |
                          v
                    Next.js + TS
                          |
                        Vercel
                          |
          +---------------+----------------+
          |                                |
          v                                v
       Supabase                           n8n
  +--------+---------+              automatizaciones
  |        |         |                periféricas
Postgres  Auth     Storage
  |        |         |
  |       RLS        +------> R2 (backup/archivo/volumen)
  |
  +--> modelo canónico

WordPress -> blog / flujo editorial
```

## Principios
1. Código como activo principal y versionado.
2. Supabase como sistema de registro.
3. Seguridad también en RLS.
4. Archivos fuera de PostgreSQL.
5. n8n para periférico, no core.
6. WordPress se mantiene mientras aporte comodidad.
7. Migración gradual y reversible.

## Entornos
Definir local, previews por PR, staging privado y producción. El .es puede servir de staging si conviene, siempre fuera de indexación y sin usuarios reales.

## Archivos
Supabase Storage primario; buckets privados y URLs temporales para documentación sensible; R2 como segunda capa a concretar.
