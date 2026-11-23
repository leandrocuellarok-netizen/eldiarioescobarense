# Especificación del directorio local — v1

**Fecha:** 23/11/2026  
**Estado:** diseño técnico; no desplegado.

## Objetivo
Crear un directorio útil para residentes y empresas del partido, con filtros por localidad, rubro y tipo de servicio. El directorio debe servir como producto editorial y como inventario comercial, sin confundir inclusión básica con publicidad paga.

## Taxonomía territorial
- Belén de Escobar
- Garín
- Ingeniero Maschwitz
- Maquinista Savio
- Matheu
- Loma Verde

## Campos mínimos por ficha
| Campo | Regla |
|---|---|
| id | Identificador estable |
| nombre | Denominación pública del comercio/organización |
| slug | URL legible |
| localidad | Una de las seis localidades; admitir “por confirmar” |
| rubro | Categoría normalizada |
| descripción | Texto factual y breve, sin elogios no sustentados |
| dirección | Solo si está corroborada |
| teléfono / email | Solo canales públicos verificados |
| sitio / redes | Enlaces oficiales comprobados |
| fuente | URL o referencia documental |
| fecha_verificación | Fecha de la última comprobación |
| estado_verificación | pendiente / parcial / corroborado |
| estado_comercial | no prospectado / prospecto / contacto autorizado / cliente |
| patrocinado | booleano, solo con acuerdo vigente |
| actualizado_en | Fecha de modificación |

## Reglas de producto
- La ficha orgánica no debe desaparecer por no contratar publicidad.
- Los resultados patrocinados deben llevar etiqueta visible y no alterar silenciosamente la clasificación editorial.
- No publicar datos personales de titulares o empleados; usar canales comerciales públicos.
- Permitir reportar correcciones y registrar historial de cambios.
- Evitar reseñas no moderadas y afirmaciones de calidad no verificadas.
- No exponer direcciones imprecisas como si fueran exactas.

## Arquitectura de navegación
Directorio → localidad → rubro → ficha.  
Cada página de localidad incluye una breve guía territorial, categorías y fecha de actualización.  
Cada ficha muestra fuente, fecha de verificación y canal oficial, cuando exista.

## SEO local
- Título único por localidad y categoría.
- Datos estructurados LocalBusiness solo cuando los campos requeridos estén verificados.
- Canonical por ficha.
- Sitemap con fichas públicas corroboradas.
- No indexar fichas incompletas, duplicadas o no verificadas.

## Próxima implementación
1. Definir esquema JSON.
2. Cargar un lote piloto pequeño con fichas verificadas.
3. Probar filtros y navegación móvil.
4. Agregar formulario de corrección.
5. Revisar privacidad, términos y política de patrocinio antes de abrir el directorio.
