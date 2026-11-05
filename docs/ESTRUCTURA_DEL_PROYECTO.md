# Estructura del proyecto

```text
enoe-mercado-laboral-mexico-2006-2026/
├── data/
│   ├── MANIFIESTO_DATOS.csv
│   ├── geo/
│   │   └── entidades_federativas.geojson                 # Mega
│   ├── parquet/
│   │   └── historical/
│   │       └── enoe_analisis_pl_2006T1_2026T1.parquet   # Mega
│   └── raw/
│       ├── INPC/                                        # Mega
│       ├── lpei/                                        # Mega; pipeline complementario
│       ├── lp/                                          # Mega; pipeline complementario
│       └── salarios_minimos/                            # Mega
├── docs/
│   ├── DATOS_Y_REPLICACION.md
│   └── ESTRUCTURA_DEL_PROYECTO.md
├── notebooks/
│   └── Exploracion_ENOE_reorganizado.ipynb              # próxima entrega
├── outputs/                                             # generado al ejecutar
├── .gitignore
├── LICENSE                                              # MIT: código
├── LICENSE-CONTENT.md                                   # CC BY-SA 4.0: contenido
├── README.md
└── requirements.txt
```

## Qué se versiona

Se versionan el cuaderno, el código auxiliar, los manifiestos, la documentación y los archivos de configuración necesarios para replicar la lógica analítica.

## Qué se distribuye por Mega

Se distribuyen por Mega los Parquet, archivos comprimidos de microdatos, archivos auxiliares de gran tamaño, archivos tabulares fuente y el GeoJSON. No se suben a GitHub para evitar duplicar archivos pesados y porque el repositorio no pretende sustituir los portales oficiales de datos.

## Qué se genera localmente

La carpeta `outputs/` contiene tablas, gráficos, mapas y productos intermedios emitidos al ejecutar el cuaderno. Puede eliminarse y regenerarse sin perder el código ni los insumos.
