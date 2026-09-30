# ADR-001 · Backend principal: Supabase
- **Estado:** Aceptado como dirección objetivo.
- **Fecha:** 30/09/2026

## Decisión
Adoptar Supabase como backend objetivo: PostgreSQL + Auth + RLS + Storage.

## Consecuencias
El modelo de datos será central y versionado; la seguridad se expresará también en RLS; Xano se auditará y migrará, no se reactivará como destino.
