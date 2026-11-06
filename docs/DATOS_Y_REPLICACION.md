# Datos y reproducción

## Propósito

Este repositorio contiene el código y la documentación del análisis exploratorio **El trabajo en México: ¿cómo vamos?**. Para mantenerlo ágil y permitir una descarga realista, los microdatos procesados y los insumos de mayor tamaño se distribuyen fuera de GitHub.

## Datos y publicaciones

El paquete de datos de reproducción se encuentra en:

> [Descargar la carpeta de datos en Mega](https://mega.nz/folder/RtVilTqL#HwadnXj5Ch8BmGkU55xvfw)

Las publicaciones asociadas son:

- [Informe de divulgación: El trabajo en México: ¿Cómo vamos?](https://mega.nz/file/QhslzRYT#SRwd_2eC5XUHmsQj1ioO9pJHwnVP6ZK03iWgrdw_MBo)
- [Cuaderno técnico: El trabajo en México: ¿Cómo vamos?](https://mega.nz/file/hlEV0QKb#sGArTPMjkYwCjeFQOhi2WpPcNq_W1j0bjpIRLk7DzJM)

## Qué debe descargarse

Descarga la carpeta `data/` desde Mega y fusiónala con la carpeta `data/` del repositorio clonado. Conserva las rutas y nombres de archivo del [manifiesto](../data/MANIFIESTO_DATOS.csv).

El insumo central es:

```text
data/parquet/historical/enoe_analisis_pl_2006T1_2026T1.parquet
```

También se requieren el GeoJSON de entidades federativas, el archivo del INPC y la serie de salario mínimo para reproducir mapas, deflactación e índice de Kaitz.

## Pasos de reproducción

1. Clona el repositorio.

   ```bash
   git clone https://github.com/DevArmando99/enoe-mercado-laboral-mexico-2006-2026.git
   cd enoe-mercado-laboral-mexico-2006-2026
   ```

2. Descarga desde Mega la carpeta `data/` y fusiónala con la carpeta `data/` del repositorio. No cambies las rutas ni los nombres de los archivos.

3. Crea y activa un entorno virtual.

   **Windows (CMD):**

   ```bat
   py -m venv .venv
   .venv\\Scripts\\activate
   ```

   **macOS/Linux:**

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

4. Instala las dependencias.

   ```bash
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

5. Inicia Jupyter desde la raíz del repositorio y abre el cuaderno.

   ```bash
   jupyter lab
   ```

   El cuaderno se encuentra en `notebooks/Exploracion_ENOE.ipynb`. Ejecútalo de arriba hacia abajo. Si el cuaderno usa rutas relativas con `Path.cwd()`, el kernel debe iniciarse desde la raíz del repositorio.

## Alcance de la reproducción

- Periodo: 2006T1–2026T1.
- 2026 corresponde exclusivamente a T1.
- 2020T2 se excluye porque no se levantó la ENOE habitual.
- Las estimaciones descriptivas usan el factor trimestral de expansión válido.
- Los montos monetarios se deflactan a pesos de 2026T1.
- Los productos se escriben en `outputs/`; no se versionan.

## Procedencia y responsabilidad

Los microdatos de base provienen de fuentes públicas de INEGI. El procesamiento, las decisiones analíticas, el código, las visualizaciones y las interpretaciones son responsabilidad del autor. Este repositorio es una investigación independiente y **no es una publicación oficial del INEGI**.

Consulta el programa oficial de la [ENOE](https://www.inegi.org.mx/programas/enoe/15ymas/) y las fichas metodológicas vigentes antes de reutilizar resultados con fines analíticos o de política pública.
