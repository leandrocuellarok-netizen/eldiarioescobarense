# Modelo de datos del directorio local — v2

**Fecha:** 23/11/2026  
**Estado:** especificación interna.

## Objetivo

Construir un directorio útil para lectores y una herramienta comercial auditable para La Gaceta de Escobar. La ficha básica debe poder existir sin que el comercio contrate publicidad.

## Entidades

### Comercio / organización

- `id`: identificador interno estable.
- `nombre_publico`: nombre comercial o institucional.
- `razon_social`: opcional; solo si una fuente pública fiable la confirma.
- `localidad`: una de Belén de Escobar, Garín, Ingeniero Maschwitz, Maquinista Savio, Matheu o Loma Verde.
- `direccion_publica`: domicilio comercial o sede pública.
- `rubro`: categoría principal y etiquetas secundarias.
- `descripcion_neutral`: descripción factual, no promocional.
- `web_oficial`, `redes_oficiales`: URLs verificadas.
- `contacto_comercial_publico`: canal empresarial publicado; nunca inferir emails.
- `fuentes[]`: URL, título, editor, fecha de publicación, fecha de consulta y dato respaldado.
- `verificado_en`: fecha de última comprobación.
- `estado_ficha`: descubierta, datos_parciales, actividad_verificada, dirección_verificada, lista_para_revision, publicada.
- `estado_comercial`: no_evaluado, prospecto, canal_publico_identificado, propuesta_autorizada, anunciante_contrato_vigente, inactivo.
- `consentimiento_promocional`: pendiente, otorgado, rechazado, vencido.
- `notas_revision`: discrepancias y tareas pendientes.

## Reglas de integridad

1. No publicar una dirección solo porque aparece en una ficha de mapas: contrastarla con web oficial, directorio institucional o confirmación del establecimiento.
2. Si la empresa tiene varias sedes, registrar cada sede por separado.
3. No asignar a Garín una empresa de Olivos ni a Loma Verde una dirección de Belén sin explicar la referencia territorial.
4. No usar reseñas de usuarios como prueba de facturación, calidad certificada, empleo o solvencia.
5. No convertir anuncios de inversión en resultados ya ejecutados.
6. La ficha gratuita y la contratación publicitaria son procesos independientes.
7. El rótulo “destacado” debe indicar que existe una contraprestación comercial.
8. Conservar el historial de cambios y la fuente de cada dato.

## Filtros de la interfaz

- Localidad.
- Rubro.
- Tipo de organización: comercio, pyme, industria, institución, profesional, paseo comercial.
- Servicios / etiquetas.
- Ficha verificada o pendiente de actualización.

## Reglas de orden

- Resultados orgánicos por coincidencia de rubro y localidad.
- Los espacios pagos se muestran en módulos separados e identificados como “Publicidad” o “Comercio destacado”.
- No permitir que el pago modifique la cobertura editorial ni la posición de una noticia.

## SEO y accesibilidad

- URL legible por ficha: `/directorio/localidad/rubro/nombre`.
- Título y descripción únicos.
- Datos estructurados LocalBusiness u Organization solo cuando los campos estén comprobados.
- Enlaces descriptivos, imágenes con texto alternativo y navegación por teclado.
- No indexar fichas incompletas, duplicadas o con datos desactualizados.

## Próximo paso técnico

Implementar un archivo de datos estructurado y una vista de directorio que lea estos campos. Mantener las fichas en estado borrador hasta completar la verificación y la aprobación editorial.
