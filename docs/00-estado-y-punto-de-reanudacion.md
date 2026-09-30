# 00 · Estado y punto de reanudación

**Fecha de corte:** 30/09/2026  
**Estado:** pausa controlada / documentación de continuidad

## Estado real
- Producción: **tuformacionimporta.com** sobre WordPress + Airtable + trabajo manual.
- Blog: WordPress, con publicación recurrente orientada a captación y SEO.
- Desarrollo previo: **tuformacionimporta.es** como acceso interno al proyecto WeWeb; no se desea tráfico ni usuarios reales.
- WeWeb: referencia funcional/visual. Inventario verificado: **32 páginas, 8 componentes no-code y 37 variables globales**.
- Xano: apagado; no será runtime futuro, pero debe auditarse en detalle.
- Existe un modelo relacional histórico trabajado previamente para desarrolladores.

## Decisiones
1. Frontend objetivo: **Next.js + TypeScript**.
2. Repositorio: **GitHub**.
3. Deploy: **Vercel**.
4. Backend: **Supabase** (PostgreSQL, Auth, RLS y Storage).
5. WordPress se mantiene inicialmente como flujo editorial.
6. n8n se reserva para automatizaciones periféricas.
7. Supabase Storage será el almacenamiento primario; Cloudflare R2 se contempla como segunda capa.
8. Xano se audita como fuente histórica, no como plataforma de destino.

## Pendiente
- Visión detallada del producto.
- Auditoría Xano.
- Revisión del modelo relacional histórico.
- Auditoría Airtable y procesos manuales.
- Auditoría SEO con Search Console, GA4, WordPress y crawl.
- Modelo canónico Supabase.
- Alcance exacto de la primera versión en código.

## Punto exacto de reanudación
1. Completar visión funcional y de negocio.
2. Auditar Xano.
3. Revisar modelo relacional histórico.
4. Auditar Airtable y procesos manuales.
5. Analizar Search Console, GA4 y WordPress.
6. Contrastar visión + Xano + modelo histórico + Airtable + WeWeb.
7. Diseñar modelo canónico Supabase, RLS, Storage y migración.
8. Definir release de sustitución y criterios de corte.
9. Solo entonces iniciar el desarrollo Next.js.
