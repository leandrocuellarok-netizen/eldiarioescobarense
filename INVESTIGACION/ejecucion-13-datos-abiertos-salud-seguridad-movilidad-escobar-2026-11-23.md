# Investigación 13 — Datos abiertos, salud, seguridad y movilidad de Escobar

**Fecha de consulta:** 23 de noviembre de 2026  
**Ámbito:** Partido de Escobar  
**Estado:** investigación interna. No publicar sin revisión editorial.

## 1. Hallazgo central: el portal municipal de datos abiertos

El portal oficial informa **53 datasets en 15 categorías**. La clasificación publicada incluye 1 dataset de Seguridad, 4 de Salud, 9 de Movilidad y Tránsito y 10 de Infraestructura y Servicios Públicos.

Fuente: https://datos.escobar.gob.ar/

Este catálogo permite pasar de una investigación basada solamente en notas y directorios a una base territorial reproducible. Sin embargo, la existencia de un dataset no significa que esté actualizado al día ni que mida el fenómeno que el título podría sugerir.

## 2. Seguridad: distinguir infraestructura de delitos

### Dataset municipal disponible

El único recurso clasificado en la categoría Seguridad se titula **Instalaciones de Seguridad del Partido de Escobar**. Contiene localización geográfica de comisarías, subcomisarías, destacamentos, jefaturas, centros de monitoreo, garitas y postas.

- Fuente: relevamiento propio del Municipio.
- Creación: 01/10/2025.
- Última actualización declarada: 31/03/2026.
- Periodicidad declarada: anual.
- Formatos: GeoJSON y Shapefile.
- Licencia: Open Data Commons Open Database License (ODbL).

Ficha: https://datos.escobar.gob.ar/dataset/instalaciones-de-seguridad-del-partido-de-escobar

**Límite:** este archivo cartografía instalaciones institucionales; no contiene denuncias ni hechos delictivos. No permite determinar qué barrio es más o menos seguro.

### Indicadores operativos informados por el Municipio

La página municipal de Seguridad informa 2.100 cámaras, 426 km de fibra óptica, 182 móviles policiales, 58.000 personas conectadas a Ojos y Oídos en Alerta, 1.452 alarmas vecinales y 86 paradas seguras. También informa 107.396 actuaciones de la Policía Municipal desde su creación el 14/03/2025, un promedio de demora de 6 minutos y una reducción del 40% en el tiempo de respuesta.

Fuente: https://www.escobar.gob.ar/municipio/seguridad/

Estos son indicadores operativos y cifras comunicadas por el propio Municipio. No equivalen a una tasa de delitos, no miden victimización y no cuentan con una serie temporal homogénea expuesta en esa página. Para cualquier nota deben atribuirse expresamente al Municipio y solicitarse metodología, periodo de corte y definición de cada indicador.

### Estadística criminal oficial

El SNIC publica bases nacionales y departamentales desde 2000/2014, manual de usuario y glosario delictual. La ficha nacional fue actualizada el 31/05/2026 y la página oficial informa evaluación de calidad estadística tipo A otorgada por el centro de excelencia de UNODC.

- Portal oficial: https://www.argentina.gob.ar/seguridad/estadisticascriminales
- Catálogo de datos: https://www.datos.gob.ar/dataset/seguridad-snic---total-pais-estadisticas-criminales-republica-argentina
- Dataset departamental: https://www.datos.gob.ar/dataset/seguridad-snic---departamental-estadisticas-criminales-republica-argentina-por-departamentos

Un tablero secundario que declara procesar datos SNIC muestra para Escobar 4.586 hechos registrados en 2025, 9 homicidios dolosos, 1.078 robos y 1.169 hurtos. Es una pista de análisis, no una cifra lista para publicar: falta reproducir el filtro directamente desde el archivo primario, revisar códigos, población de referencia y comparabilidad interanual.

Tablero secundario: https://inseguridad.vercel.app/inseguridad/buenos-aires/escobar

**Criterio editorial:** no publicar mapas de delitos por barrio hasta contar con fuente primaria, geografía y periodo verificables. No calificar barrios enteros como peligrosos o seguros. No mapear domicilios particulares ni ubicaciones que expongan a víctimas.

## 3. Salud: inventario y límites temporales

La página municipal informa **8 hospitales, 4 Unidades de Diagnóstico Precoz (UDP) y 18 CAPS**. La cartilla permite consultar centros por localidad, guardias, prestaciones y horarios.

- Centros de salud: https://www.escobar.gob.ar/municipio/centros-de-salud/
- Guardias: https://www.escobar.gob.ar/municipio/guardias-y-farmacias/
- Salud mental y adicciones: https://www.escobar.gob.ar/municipio/cartilla-de-salud-mental-y-adicciones/

El portal de datos abiertos tiene cuatro recursos de Salud:
1. Centros de Salud del Partido de Escobar (GeoJSON y SHP).
2. Estadísticas Vitales 2005–2022 (XLSX).
3. Farmacias Escobar (XLSX).
4. Centros Médicos Unificado Escobar, versión completa (XLSX).

Fichas:
- https://datos.escobar.gob.ar/dataset/centros-de-salud-del-partido-de-escobar
- https://datos.escobar.gob.ar/dataset/estadisticas-vitales-2005-2022-escobar

Los recursos geográficos de centros de salud declaran actualización al 31/03/2026. El dataset de estadísticas vitales cubre 2005–2022: no debe presentarse como estadística sanitaria actual de 2026.

**Brecha detectada:** la cartilla web muestra filtros para Belén, Garín, Ingeniero Maschwitz, Maquinista Savio, Matheu y Loma Verde, pero no presenta 24 de Febrero como filtro independiente. Hay que aclarar si los servicios de esa jurisdicción están incluidos bajo otra localidad o si falta cobertura en la clasificación.

## 4. Movilidad, calles e infraestructura urbana

El portal incluye:
- Líneas y paradas de colectivo del Partido de Escobar 2026 (XLSX).
- Estaciones y línea ferroviaria.
- Paradas Mi Bus.
- Paradas Seguras.
- Terminal de ómnibus.
- Ejes de calles del partido (GeoJSON y SHP).

Ficha de colectivos: https://datos.escobar.gob.ar/dataset/lineas-y-paradas-de-colectivo-del-partido-de-escobar-2026  
Ficha de ejes de calles: https://datos.escobar.gob.ar/dataset/ejes-de-calles-del-partido-de-escobar

También existen capas de cobertura de agua potable y red cloacal basadas en información de AySA correspondiente a **2016**. Son útiles como antecedente histórico de infraestructura, pero demasiado antiguas para describir cobertura actual sin actualización.

**Aplicación editorial:** cruzar paradas, centros de salud, escuelas y equipamientos públicos para estudiar accesibilidad por localidad, dejando explícito el año de cada capa. No inferir tiempos reales de viaje sin datos operativos.

## 5. Comercio local: fuente primaria municipal

El directorio municipal informa **219 comercios en 13 rubros** y ofrece filtros para seis localidades: Belén de Escobar, Garín, Ingeniero Maschwitz, Maquinista Savio, Matheu y Loma Verde.

Fuente: https://www.escobar.gob.ar/municipio/comercios-locales/

Es la mejor base pública inicial para prospectar y construir el directorio de La Gaceta. No es un padrón exhaustivo de toda la actividad económica, no certifica que cada negocio siga abierto y no incluye 24 de Febrero como filtro independiente.

## 6. Próximas tareas verificables

1. Descargar y versionar los GeoJSON de seguridad y salud, registrando fecha y licencia.
2. Obtener la base SNIC y reproducir los indicadores del tablero secundario para Escobar y municipios comparables.
3. Revisar códigos delictuales y población usada para tasas por 100.000 habitantes.
4. Construir una matriz de accesibilidad a centros de salud con paradas y líneas 2026.
5. Solicitar por acceso a la información pública series municipales de delitos, actuaciones y tiempos de respuesta, con definiciones y periodos.
6. Reconciliar la nomenclatura de las siete localidades y la ausencia de 24 de Febrero en algunos filtros municipales.

## 7. Regla de publicación

Todos los datos de este documento son insumos internos. La información de seguridad, salud y comercios requiere revisión de vigencia, metodología, privacidad y atribución antes de cualquier publicación. No se contactó a personas ni se enviaron consultas en esta ejecución.
