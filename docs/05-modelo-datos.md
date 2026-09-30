# 05 · Modelo de datos

**Estado: no existe todavía un modelo canónico aprobado para Supabase.**

## Fuentes a reconciliar
1. Visión futura.
2. Modelo relacional histórico.
3. Xano.
4. Airtable.
5. WeWeb.
6. Procesos manuales.

## Dominios preliminares
Identidad/auth, perfil/persona, entidades, cursos, ediciones/ofertas, convocatorias, solicitudes/inscripciones, favoritos si se confirma, documentos, comunicaciones, auditoría, geografía y taxonomías.

## Principios
- IDs internos estables y conservación de IDs legacy.
- Normalizar el núcleo de negocio.
- Estados de proceso modelados conscientemente.
- RLS diseñada junto con el esquema.
- Archivos fuera de PostgreSQL.
- Minimización y trazabilidad de datos personales.
- Índices/constraints por casos de uso reales.

## Entregables
ERD, diccionario, matriz fuente→destino, deduplicación, IDs legacy, RLS y plan de migración/validación.
