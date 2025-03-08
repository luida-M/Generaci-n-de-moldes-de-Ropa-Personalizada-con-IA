# Trabajo Final: "Generación de Moldes de Ropa personalizados con IA"

#### Comisión: 71950   

#### Alumno: Luida Medina

### Versión: 2.0

# Definición del Problema:
Generación_de_Molde_Personalizada_con_IA

## 1. Problemática
#### Contexto
En la industria textil, la creación de moldes y patrones para prendas personalizadas es un proceso complejo que requiere conocimientos técnicos y herramientas especializadas. Muchos usuarios que no disponen de software específico o experiencia en patronaje digital encuentran dificultades para generar diseños precisos y adaptados a sus necesidades.

### Problema
El método tradicional de diseño manual de moldes implica el uso de herramientas de diseño vectorial y conocimientos avanzados en patronaje. Esto no solo ralentiza el proceso, sino que también limita la capacidad de personalizar los diseños para adaptarse a medidas específicas o tendencias actuales.

### Solución
Se propone automatizar la generación de moldes y patrones utilizando inteligencia artificial generativa y técnicas de prompt engineering. Esta solución permitirá:
* Calcular medidas básicas para diferentes tipos de prendas (camisa, pantalón, vestido) según tallas predefinidas, y también aceptar medidas personalizadas.
* Generar imágenes completas de la prenda y patrones detallados de cada una de sus partes (por ejemplo, frente, espalda, manga, cuello, etc.).
* Utilizar la API de OpenAI (DALL·E) para crear imágenes de alta calidad de forma automatizada.
* Proporcionar prompts e instrucciones detalladas para la generación manual de imágenes en plataformas como NightCafe o Leonardo.ai, en caso de preferir o necesitar un método alternativo.

## 2. Metodología
### Procedimientos
####1. Cálculo de Medidas:

* Se implementan funciones que calculan medidas básicas para cada prenda y talla (por ejemplo, para camisa, pantalón y vestido).
* Se ofrece la opción de ingresar medidas personalizadas para adaptar el diseño a las necesidades del usuario.
  
#### 2. Generación Automatizada de Imágenes:
* Se utiliza la API de OpenAI para generar imágenes a partir de prompts diseñados específicamente para mostrar la prenda completa o sus piezas por separado.
* Las imágenes generadas se descargan, muestran al usuario y se guardan en Google Drive.
  
##### 3. Generación de Patrones Detallados:

*Se crean funciones que generan prompts para obtener imágenes de las distintas partes de la prenda (frente, espalda, manga, cuello, etc.), incorporando las medidas relevantes.

#### 4. Prompts e Instrucciones para Uso Manual:
* Se desarrollan prompts optimizados y se ofrecen instrucciones detalladas para que el usuario pueda utilizar manualmente plataformas como NightCafe o Leonardo.ai en caso de optar por no usar la API de OpenAI.
  
#### 5. Interacción con el Usuario:
* Se implementa una función principal que solicita al usuario el tipo de prenda, la talla y, opcionalmente, medidas personalizadas. Con estos datos se genera la imagen completa y los patrones de las piezas por separado.

## Justificación:
Este enfoque permite automatizar y simplificar el proceso de creación de moldes, haciendo posible la personalización y agilizando el diseño de prendas. La integración de IA y prompt engineering mejora la precisión de los patrones y abre la puerta a nuevas formas de diseño accesibles para usuarios sin conocimientos técnicos avanzados.

## 3. Herramientas y Tecnologías
* Lenguaje de Programación: Python
* API de OpenAI (DALL·E): Utilizada para la generación automatizada de imágenes de moldes y patrones.
* Plataformas Alternativas:
** NightCafe y Leonardo.ai: Se ofrecen instrucciones y prompts para generar imágenes manualmente en estas plataformas.
* Técnicas de Prompt Engineering:
** Desarrollo de prompts detallados que incluyen descripciones precisas, medidas, y términos técnicos (por ejemplo, "dibujo técnico, estilo vectorial, monocromo") para mejorar la calidad y precisión de las imágenes.
* Almacenamiento: Google Drive, para guardar las imágenes generadas.

4. Implementación
El código desarrollado integra las siguientes funcionalidades:

* Cálculo de Medidas: Funciones que devuelven medidas predeterminadas para cada tipo de prenda y talla, además de permitir la entrada de medidas personalizadas según la preferencia del usuario.

* Generación de Imágenes con API: Funciones que utilizan la API de OpenAI para generar imágenes de la prenda completa y de sus componentes. El proceso incluye:

** Creación del prompt adecuado.
** Solicitud de imagen a la API.
** Descarga, visualización y guardado de la imagen en Google Drive.
* Generación de Patrones Separados: Se generan imágenes individuales para cada parte de la prenda (como frente, espalda, manga y cuello en el caso de una camisa; o delantero, trasero y pierna en pantalón) mediante prompts específicos que incluyen las medidas correspondientes.

* Generación de Prompts Alternativos e Instrucciones Manuales: Funciones adicionales que generan prompts optimizados e incluyen instrucciones para usar NightCafe o Leonardo.ai de forma manual, permitiendo al usuario tener una opción alternativa a la generación automatizada mediante OpenAI.

* Interfaz de Usuario: La función principal solicita al usuario que elija el tipo de prenda, talla y la opción de usar medidas personalizadas, para luego coordinar la generación de la imagen completa y de cada patrón individual.


Google Colab:
   ```bash
https://colab.research.google.com/drive/1MNZhzhxaGm3NkY88CZFA-4UEgroVoFYp?usp=sharing

