# Arquitectura web v1 — La Gaceta de Escobar

**Estado:** especificación preliminar, no implementada.  
**Objetivo:** lanzar una web rápida, indexable, fácil de actualizar y con espacios comerciales administrables.

## 1. Portada
1. Franja superior: fecha, localidades, contacto editorial y redes.
2. Cabecera: logotipo, bajada y menú principal.
3. Titular principal con imagen, sección, fecha y firma.
4. Dos o tres noticias secundarias.
5. Módulo “Últimas noticias”.
6. Bloque “Empresas y economía”.
7. Bloque “Industria y empleo”.
8. Bloque “La Gaceta en tu localidad”, con seis accesos.
9. Directorio comercial.
10. Agenda y oportunidades de empleo.
11. Newsletter.
12. Pie con información institucional, política de correcciones, publicidad y contacto.

## 2. Navegación
- Portada
- Últimas noticias
- Economía y empresas
- Industria
- Comercio local
- Empleo y formación
- Política y gestión
- Sociedad
- Educación
- Cultura y agenda
- Deportes
- Opinión
- Localidades: Belén, Garín, Ingeniero Maschwitz, Maquinista Savio, Matheu y Loma Verde

## 3. Páginas y rutas sugeridas
- `/` portada
- `/actualidad/`
- `/economia/`
- `/empresas/`
- `/industria/`
- `/empleo/`
- `/comercios/`
- `/agenda/`
- `/localidades/garin/` (y una página equivalente por localidad)
- `/autor/`
- `/publicidad/`
- `/contacto/`
- `/politica-editorial/`

## 4. Ficha de noticia
Cada publicación debe tener: título, bajada, cuerpo, sección, localidad, autor, fecha de publicación, fecha de actualización, imagen con crédito, fuentes, etiquetas, estado de verificación y tipo de contenido (editorial, opinión o patrocinado).

## 5. Directorio comercial
Campos mínimos: nombre comercial, rubro, localidad, dirección, web o canal público, descripción breve, fuente, fecha de consulta, estado de verificación y consentimiento para destacar información aportada directamente por el comercio.

No convertir el directorio público municipal en una lista de anunciantes confirmados. La ficha básica y la pauta publicitaria deben estar separadas.

## 6. Espacios comerciales
- Banner cabecera (con límites de peso y dimensiones).
- Banner lateral o intermedio.
- Módulo “Empresa destacada”.
- Patrocinio del newsletter.
- Especial comercial claramente rotulado.
- Directorio destacado.

Todos los espacios deben indicar “Publicidad” o “Contenido patrocinado”. La contratación no otorga control sobre la cobertura periodística.

## 7. Tecnología recomendada para el MVP
- Astro como generador de sitio estático.
- Markdown para noticias y páginas editoriales.
- JSON para el directorio comercial y la agenda.
- GitHub como repositorio y control de versiones.
- GitHub Pages como primera opción de publicación estática, sujeto a configurar dominio y despliegue.
- Analítica respetuosa de privacidad y Search Console una vez publicado.

Ventaja: bajo costo operativo, rendimiento y control editorial. Límite: para edición no técnica se necesitará luego un CMS conectado al repositorio. No se debe anunciar que existe un panel de administración hasta implementarlo.

## 8. Flujo de publicación
Idea → fuente primaria → verificación → borrador → edición → revisión de datos y derechos → aprobación humana → publicación → distribución → seguimiento/corrección.

## 9. SEO y rendimiento
- Una URL canónica por nota.
- Títulos y descripciones únicos.
- Datos estructurados NewsArticle, Organization y BreadcrumbList cuando corresponda.
- Sitemap XML, robots.txt, Open Graph y tarjetas sociales.
- Imágenes WebP/AVIF con texto alternativo y crédito.
- Diseño responsive, contraste AA y navegación por teclado.
- Evitar titulares engañosos, contenido duplicado y páginas de localidad vacías.

## 10. Etapas de construcción
1. Identidad y prototipo de portada.
2. Estructura de navegación y plantillas.
3. Carga de primeras 10 notas verificadas.
4. Directorio inicial con registros de fuente comprobable.
5. Espacios publicitarios y página de tarifas.
6. Pruebas móviles, SEO y accesibilidad.
7. Publicación y medición.

**Pendiente antes de programar:** confirmar dominio, plataforma final, correo editorial, responsables de firma y política de comentarios.
