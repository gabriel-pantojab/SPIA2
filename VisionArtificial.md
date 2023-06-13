# Visión Artificial

[Atras](./README.md)

[comment]: <> (menu)

- [Visión Artificial](#visión-artificial)
  - [Historia](#historia)
  - [Aprendizaje Automático](#aprendizaje-automático)
    - [Procesamiento de Imágenes](#procesamiento-de-imágenes)
    - [Transformaciones Morfológicas](#transformaciones-morfológicas)
      - [Dilación Binaria](#dilación-binaria)

Desarrolla algoritmos y sistemas que permiten a las computadoras "ver" y entender imagenes y videos.

**Proceso Básico:**

1. Adquisición de datos a través de una cámara u otros dispositivos.
2. Extraer información de esos datos con algoritmos de procesamiento de imágenes y aprendizaje automático.

## Historia
- 1950: uso de computadoras para analizar imagenes y extraer información, pero era de forma manual.
- 1960: se desarrollan algoritmos para procesar imagenes, técnicas de segmentación y detección de bordes.
- 1970: técnicas de reconocimiento de patrones y uso de la inteligencia artificial.
- 1980: primeros sistemas comerciales principalmente para el control de calidad.
- 1990: técnicas avanzadas como visión estéreo y visión 3D, tambien se desarrollan sistemas de reconocimiento de facial.
- 2000: importantes avances en el aprendizaje automático que permiten el desarrollo de sistemas de visión artificial más complejos.

## Aprendizaje Automático

En lugar de programar reglas para reconocer patrones podemos dejar que la computadora aprenda a reconocer estos patrones a partir de ejemplos.

### Procesamiento de Imágenes

1. **Adquisición de imágenes:** capturar imágenes con una cámara, escanear.
2. **Preprocesamiento:** mejorar la calidad de la imagen, eliminar ruido, mejorar contraste, etc.
3. **Segmentación:** identificar regiones de interes, mediante técnicas de umbralización, detección de bordes, etc.

### Transformaciones Morfológicas

Las transformaciones morfológicas se encargan de cambiar la forma y estructura de los objetos. Permiten obtener una idea de la estructura y forma de los objetos en una imagen.

#### Dilación Binaria

Dados dos conjuntos $A$ y $B$ de $Z^2$, la dilatación denotada por $A \oplus B$ es el conjunto: $A \oplus B = {c \in E^N | c = a + b}$

La dilatación, también llamada “crecimiento”, “llenado”, “expansión”, etc., produce un efecto de engrosamiento de los bordes del objeto.