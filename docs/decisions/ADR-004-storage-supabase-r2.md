# ADR-004 · Archivos: Supabase Storage + segunda capa R2
- **Estado:** Dirección aceptada; detalle de R2 pendiente.
- **Fecha:** 30/09/2026

## Decisión
Supabase Storage será el almacenamiento principal. Documentación sensible en buckets privados. Cloudflare R2 se contempla para backup, archivo histórico y/o gran volumen.

## Consecuencias
PostgreSQL guarda metadatos, no binarios. Deben definirse backup, retención, borrado, restauración y validación de archivos.
