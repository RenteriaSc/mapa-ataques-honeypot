# Proyecto: Mapa de ataques hacker reales (DataXperience - Universidad EAN)

## Contexto
Soy Sebas, estudiante de Ingeniería de Sistemas y programador junior; quiero dedicarme a la ciberseguridad.
Este es mi proyecto final del curso de Ciencia de Datos. Lo hago solo.
Fecha límite: 21 de noviembre de 2026, 23:59 (hora Colombia).
Dataset: AWS Honeypot Attack Data (Kaggle, casimian2000/aws-honeypot-attack-data).
Pregunta: ¿desde dónde, cuándo y contra qué servicios atacan, y se puede predecir el servicio atacado?

## Cómo trabajar conmigo
- Explícame cada paso antes de hacerlo y por qué; quiero aprender, no solo tener el código.
- Si algo no está claro, pregúntame antes de suponer. No inventes datos, columnas ni resultados.
- Trabaja por etapas y espera mi visto bueno antes de pasar a la siguiente.
- Lleva el checklist del proyecto y márcame qué falta al terminar cada sesión.

## Estructura obligatoria del repositorio
mapa-ataques-honeypot/
  README.md, datos/, notebook/, presentacion/, video/
Agrega también: requirements.txt, .gitignore (Python) y LICENSE (MIT).

## Buenas prácticas: Python y pandas
- PEP 8: nombres claros en snake_case, en español o inglés pero sin mezclar.
- Funciones pequeñas con docstring para pasos que se repiten (limpiar, graficar).
- Nada de rutas absolutas: rutas relativas o la URL raw del repositorio.
- Semilla fija (random_state=42) en todo lo aleatorio.
- No modificar el CSV original: los datos limpios se guardan aparte (datos/ataques_limpio.csv).
- Comentarios que expliquen el porqué, no el qué.

## Buenas prácticas: cuaderno de Colab
- Orden: título y descripción, índice, importaciones, carga, Etapa 1, Etapa 2, Etapa 3, conclusiones.
- Cada sección con encabezado en Markdown y una celda de texto que interprete cada resultado.
- Debe funcionar con "Ejecutar todo" desde cero en un Colab nuevo, sin errores.
- Gráficas con título, ejes con nombre y unidades, y leyenda cuando haga falta.
- Antes de subirlo, limpiar las salidas pesadas y volver a ejecutarlo completo.

## Etapas del proyecto
1. Preparación de datos (Módulo 1): explorar tipos, nulos, duplicados y errores; limpiar y documentar.
2. Análisis estadístico (Módulo 2): media, mediana, moda, rango, varianza, desviación estándar, comparar variables, outliers e hipótesis.
3. Modelo predictivo (Módulo 3): por confirmar cuando tenga el contenido del módulo.

## Buenas prácticas: estadística (Etapa 2)
- Presentar las estadísticas en tablas limpias (DataFrame redondeado a 2 decimales), no como prints sueltos.
- Elegir la medida adecuada: si hay outliers o sesgo, explicar por qué la mediana representa mejor que la media.
- Detectar outliers con la regla IQR y mostrarlos en un boxplot; explicar si son errores o ataques reales.
- Cada hipótesis debe salir de un valor concreto de las tablas, no de suposiciones.
- Debajo de cada resultado, una explicación en lenguaje sencillo pensada para un analista de seguridad.

## Buenas prácticas: modelo
- Separar entrenamiento y prueba antes de cualquier ajuste; no usar el puerto de destino como entrada (fuga de datos).
- Comparar siempre contra un modelo base (la clase más común).
- Reportar accuracy, F1 por clase y matriz de confusión; explicar qué significan.

## Buenas prácticas: Git y GitHub
- Commits pequeños y frecuentes con mensajes claros (ej.: "feat: limpieza de nulos", "docs: README etapa 1").
- Nunca subir claves, tokens ni archivos de más de 100 MB; si el CSV pesa más, comprimirlo o usar una muestra documentada.
- Repositorio público; comprobar todos los enlaces desde una ventana de incógnito.

## Buenas prácticas: README
- Título, descripción corta, pregunta del proyecto y por qué se relaciona con ciberseguridad.
- Autor, enlace al video, enlace para abrir el cuaderno en Colab (badge "Open in Colab").
- Fuente del dataset con enlace, descripción de columnas, cómo ejecutar, hallazgos principales con 2 o 3 imágenes y conclusiones.

## Buenas prácticas: presentación
- 8 a 10 diapositivas, una idea por diapositiva, gráficas grandes y poco texto.
- Exportar a PDF y guardarla en presentacion/.
