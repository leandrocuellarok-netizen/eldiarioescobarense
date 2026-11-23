# Wireframe editorial — portada v1

**Proyecto:** La Gaceta de Escobar  
**Fecha:** 23/11/2026  
**Estado:** especificación funcional preliminar; no publicada.

## Objetivo
Una portada de lectura rápida, orientada a actualidad local, economía y negocios. La prioridad es que el lector identifique qué ocurre en Escobar y que las empresas encuentren información útil sin convertir la portada en un catálogo publicitario.

## Estructura de escritorio
1. **Franja superior:** fecha, edición, acceso a localidades y redes.
2. **Masthead:** logotipo LA GACETA DE ESCOBAR, bajada “Noticias, negocios y actualidad del partido”.
3. **Navegación:** Actualidad, Economía, Empresas, Industria, Empleo, Sociedad, Localidades, Cultura, Deportes y Opinión.
4. **Titular principal:** noticia de relevancia distrital, imagen horizontal y resumen.
5. **Últimas noticias:** cuatro a seis títulos breves con hora de actualización.
6. **Radar Empresarial:** novedades de pymes, inversiones, industria, comercio y logística.
7. **Cobertura por localidad:** Belén de Escobar, Garín, Ingeniero Maschwitz, Maquinista Savio, Matheu y Loma Verde.
8. **Empleo y oportunidades:** búsquedas vigentes, convocatorias y formación, siempre con fecha de expiración.
9. **Agenda:** ferias, rondas, capacitaciones y actividades locales.
10. **Opinión y análisis:** firmas identificadas y separación de noticias.
11. **Directorio empresarial:** acceso a fichas por rubro y localidad.
12. **Newsletter:** suscripción con consentimiento explícito.
13. **Pie institucional:** quiénes somos, contacto, publicidad, política de correcciones, privacidad y condiciones.

## Estructura móvil
- Masthead compacto y menú desplegable.
- Titular principal primero.
- Últimas noticias en lista vertical.
- Acceso rápido a las seis localidades.
- Botón de búsqueda visible.
- Directorio y empleo como accesos diferenciados.
- Anuncios adaptados al ancho móvil sin tapar contenido ni simular titulares.

## Sistema publicitario
- Un banner superior claramente rotulado.
- Un módulo patrocinado dentro de Economía y Empresas.
- Fichas premium en el directorio.
- Patrocinio de newsletter.
- Publicidad contextual por localidad o rubro.

La cantidad de espacios debe limitarse para preservar velocidad y experiencia de lectura. Ninguna pieza paga puede presentarse como noticia independiente.

## Requisitos técnicos
- Diseño responsive y accesible.
- URLs legibles y permanentes por artículo.
- CMS con roles: administrador, editor, redactor y comercial.
- Estados editoriales: idea, investigación, borrador, edición, verificación, aprobado y publicado.
- Campos obligatorios: autor, fecha, localidad, sección, fuentes, estado de verificación y etiqueta comercial.
- Imágenes con crédito, licencia y texto alternativo.
- Sitemap XML, RSS, metadatos Open Graph y datos estructurados de artículos.
- Analítica con medición de páginas, fuentes de tráfico, newsletter y clics publicitarios.
- Copias de seguridad y autenticación robusta.

## Modelo de URL
- / — portada
- /actualidad/slug-de-la-noticia
- /economia/slug
- /empresas/slug
- /industria/slug
- /empleo/slug
- /localidades/garin
- /localidades/matheu
- /directorio/rubro/nombre
- /agenda/slug
- /publicidad
- /contacto
- /politica-editorial

## Criterios de publicación
No publicar automáticamente contenido generado con IA. Toda nota debe tener responsable humano, fuente verificable, fecha, revisión y estado aprobado. Los avisos de empleo y convocatorias deben llevar fecha de vigencia. Los contenidos comerciales deben estar etiquetados.

## Decisión de infraestructura pendiente
La elección entre sitio estático y CMS debe realizarse antes de crear una portada desplegable. Este documento no autoriza publicar el prototipo ni activar GitHub Pages.
