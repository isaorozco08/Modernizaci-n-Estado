Título del Proyecto
"Gobierno Digital: Análisis de Desempeño Institucional 2024 por Territorio"

Problema / Objetivo
Evaluar y comparar el desempeño de instituciones públicas colombianas en términos de transformación digital durante 2024, identificando brechas territoriales y sectorizadas en la adopción de políticas de gobierno digital.

Datos Utilizados
Fuente: Archivo Excel resultados_2024.xlsx
Estructura: 3,129 instituciones públicas x 18 variables
Cobertura geográfica: Departamentos y municipios de Colombia
Clasificación: Por rama (ejecutiva, legislativa, judicial), naturaleza jurídica, y estatus PDET
Variables principales:
Índice de Gobierno Digital (composite)
11 dimensiones temáticas (gobernanza, arquitectura, privacidad, servicios digitales, etc.)
Metodología (síntesis)
Importación y carga: Pandas, NumPy, Matplotlib, Seaborn
Limpieza inicial:
Eliminación de 4 filas de encabezados y metadatos
Estandarización de nombres de columnas (minúsculas, sin tildes)
Eliminación de columnas redundantes (IDs)
Transformación de datos:
Conversión de variables numéricas a float64 (con decimales)
Gestión de valores faltantes (NaN) mediante pd.to_numeric(errors='coerce')
Redondeo a 1 decimal
Hallazgos Clave
Alta fragmentación de datos: Las dimensiones "Proyectos de Transformación Digital" (2,470 nulos) y "Estrategias de Ciudades Inteligentes" (2,853 nulos) presentan >79% de datos faltantes, sugiriendo áreas incipientes o de reporte inconsistente.

Variabilidad institucional significativa: El índice de Gobierno Digital oscila entre 3.5 y 66.5 puntos, evidenciando disparidades profundas en madurez digital entre entidades.

Brecha en capacidades avanzadas: Dimensiones como "Innovación Pública Digital" (888 nulos) y "Servicios Ciudadanos Digitales" (1,035 nulos) muestran baja cobertura, indicando que pocas entidades han avanzado a niveles de transformación sofisticada.

Núcleo institucional fortalecido: Las dimensiones "Gobernanza", "Privacidad y Seguridad" y "Estado Abierto" tienen <5% de datos faltantes, reflejando que estas son áreas de implementación más generalizada.

Output Esperado
El notebook estructura análisis para generar:

Estadísticas descriptivas por dimensión y territorio
Visualizaciones comparativas (gráficos de distribución y territoriales)
Benchmarking departamental y por tipo de entidad
Identificación de clusters de madurez digital institucional
