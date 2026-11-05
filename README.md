# El trabajo en México: ¿cómo vamos?

**Veinte años de empleo, jornadas e ingresos**  
**ENOE · 2006T1–2026T1**

Repositorio de reproducción del análisis exploratorio del mercado laboral mexicano que acompaña el informe de divulgación *El trabajo en México: ¿cómo vamos?*. El estudio usa microdatos abiertos de la Encuesta Nacional de Ocupación y Empleo (ENOE) y expresa los ingresos reales en pesos de 2026T1.

> **Estado del repositorio:** se está preparando la infraestructura de reproducción. El cuaderno técnico y los datos se incorporarán en entregas posteriores.

## Alcance

El cuaderno reproduce indicadores descriptivos ponderados por el factor de expansión trimestral: composición ocupacional, formalidad, jornadas, ingresos laborales reales, ingreso por hora, percentiles, educación, segundo empleo y diferencias territoriales. La ENOE no permite inferir causalidad a partir de estas asociaciones descriptivas.

Los análisis excluyen 2020T2, periodo para el que la ENOE no levantó la encuesta habitual. Para 2026 se utiliza únicamente el primer trimestre.

## Qué contendrá este repositorio

- `notebooks/Exploracion_ENOE_reorganizado.ipynb`: cuaderno técnico reproducible.
- `data/`: manifiestos y documentación de los insumos; los archivos voluminosos se distribuirán mediante Mega.
- `outputs/`: carpeta de salida que generará el cuaderno.
- `docs/`: guía de reproducción, estructura, criterios metodológicos y licencias.
- `requirements.txt`: entorno Python mínimo.

## Datos y productos

Los datos no se versionan en GitHub para mantener el repositorio ligero. La carpeta de descarga en Mega y los enlaces permanentes al informe de divulgación y al **Cuaderno técnico: El trabajo en México: ¿Cómo vamos?** se agregarán cuando se publique el cuaderno definitivo.

Consulta desde ahora:

- [Guía de datos y reproducción](docs/DATOS_Y_REPLICACION.md)
- [Estructura del proyecto](docs/ESTRUCTURA_DEL_PROYECTO.md)
- [Manifiesto de insumos](data/MANIFIESTO_DATOS.csv)

## Fuentes primarias

- Instituto Nacional de Estadística y Geografía (INEGI), [Encuesta Nacional de Ocupación y Empleo](https://www.inegi.org.mx/programas/enoe/15ymas/).
- INEGI, [Índice Nacional de Precios al Consumidor](https://www.inegi.org.mx/temas/inpc/).
- Comisión Nacional de los Salarios Mínimos (CONASAMI), resoluciones y series de salario mínimo.

## Licencias

El código se distribuye bajo la [licencia MIT](LICENSE). El texto, las visualizaciones, las imágenes y el contenido editorial se distribuyen bajo [CC BY-SA 4.0](LICENSE-CONTENT.md).

## Autoría

José Armando Carreón Montañez · 2026  
Investigación independiente basada en datos abiertos. No es una publicación oficial del INEGI.
