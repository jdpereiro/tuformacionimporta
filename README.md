# TuFormacionImporta

Repositorio de continuidad, arquitectura y futuro desarrollo de **TuFormacionImporta**.

> **Estado a 30/09/2026:** proyecto en pausa controlada. El objetivo de esta documentación es poder retomar el proyecto dentro de semanas o meses exactamente desde el punto actual, sin reconstruir decisiones ni contexto.

## Punto de partida real

- **Producción actual:** `tuformacionimporta.com`, sobre WordPress + Airtable + trabajo manual del equipo.
- **Blog:** WordPress, con publicación frecuente orientada a captación y SEO. Se mantiene como flujo editorial en la arquitectura objetivo inicial.
- **Desarrollo previo:** `tuformacionimporta.es` se ha utilizado internamente para el proyecto WeWeb; no se desea tráfico ni usuarios reales por ahora.
- **WeWeb:** desarrollo avanzado que se conservará como referencia funcional y visual, no como plataforma objetivo de largo plazo.
- **Xano:** apagado. Debe auditarse en detalle porque puede contener modelo de datos, endpoints y lógica aprovechables.
- **Modelo relacional histórico:** existe documentación previa trabajada con desarrolladores y debe revisarse antes de definir el modelo canónico.

## Dirección técnica acordada

La dirección objetivo provisional es:

- Frontend: **Next.js + TypeScript**.
- Repositorio y versionado: **GitHub**.
- Despliegue: **Vercel**.
- Backend principal: **Supabase** (PostgreSQL, Auth, RLS y Storage).
- Archivos privados: **Supabase Storage** como almacenamiento primario.
- Archivo/backup/volumen masivo: **Cloudflare R2** como capa adicional a validar/implantar.
- Automatizaciones periféricas: **n8n**, evitando convertirlo en el núcleo de la lógica del producto.
- Contenido editorial: **WordPress** se mantiene inicialmente.

## No hacer al retomar

No empezar programando directamente. Antes hay que completar la visión funcional, auditar Xano, revisar el modelo relacional histórico, inventariar Airtable y estudiar Search Console/GA4/WordPress. Después se diseña el modelo canónico de Supabase y el plan de migración.

## Documentación

- [`docs/00-estado-y-punto-de-reanudacion.md`](docs/00-estado-y-punto-de-reanudacion.md)
- [`docs/01-vision-producto.md`](docs/01-vision-producto.md)
- [`docs/02-arquitectura-actual.md`](docs/02-arquitectura-actual.md)
- [`docs/03-arquitectura-objetivo.md`](docs/03-arquitectura-objetivo.md)
- [`docs/04-inventario-funcional.md`](docs/04-inventario-funcional.md)
- [`docs/05-modelo-datos.md`](docs/05-modelo-datos.md)
- [`docs/06-seo-y-wordpress.md`](docs/06-seo-y-wordpress.md)
- [`docs/07-plan-migracion.md`](docs/07-plan-migracion.md)
- [`docs/decisions/`](docs/decisions/) - decisiones de arquitectura (ADR).

## Fuente de verdad

Los documentos de este repositorio son la **fuente técnica versionada**. El Documento Maestro de Continuidad en Word es la versión cómoda de lectura humana y debe actualizarse cuando se produzcan decisiones sustanciales.
