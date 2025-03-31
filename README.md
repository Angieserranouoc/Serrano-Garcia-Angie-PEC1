# PEC 1 - Análisis de Datos Ómicos

Este repositorio contiene el trabajo realizado para la Prueba de Evaluación Continua (PEC 1) del curso de Análisis de Datos ómicos del Master Bioinformática y Bioestadística.

## Contenido

- `/data/`: Archivos de datos descargados desde Metabolomics Workbench (`.txt`).
- `/codigo/`: Código R utilizado para la exploración y análisis del dataset (formato `.Rmd`).
- `/objeto/`: Objeto `SummarizedExperiment` en formato `.Rda` que contiene la matriz de expresión y los metadatos integrados.
- `Serrano-Garcia-Angie-PEC1.pdf`: Informe final generado a partir del análisis 

## Dataset utilizado

- **ID del estudio**: ST000915
- **Fuente**: [Metabolomics Workbench](https://www.metabolomicsworkbench.org/data/DRCCMetadata.php?Mode=Study&StudyID=ST000915)
- **Descripción**:Identificación de biomarcadores metabólicos asociados a diferentes etapas de la enfermedad por hígado graso no alcohólico (NAFLD)

## Metadatos utilizados

Los metadatos utilizados en este análisis corresponden al diagnóstico clínico asociado a cada una de las muestras biológicas incluidas en el estudio ST000915. Estos diagnósticos incluyen: Normal, Steatosis, NASH (esteatohepatitis no alcohólica) y Cirrhosis.
Esta información fue extraída de la primera fila del bloque de datos que inicia en la linea 263, del archivo `ST000915_AN001490.txt` y fue utilizada para construir la columna `Diagnosis` en el objeto `SummarizedExperiment`. Su inclusión permite analizar los perfiles metabólicos en función del estado clínico del paciente, facilitando la comparación entre grupos y la exploración de patrones relacionados con la progresión de la enfermedad hepática grasa no alcohólica (NAFLD).
Los metadatos fueron fundamentales para contextualizar los resultados del análisis exploratorio, permitiendo observar cómo los perfiles metabólicos varían según el estado clínico. Aunque en esta PEC se utilizó únicamente la variable de diagnóstico, el archivo original contiene potencialmente otros factores que podrían enriquecer futuros análisis si se integran adecuadamente (por ejemplo, edad, sexo u otras variables clínicas).


## Autor

Angie Yarlady Serrano García 
Curso: Análisis de datos ómicos
Universidad: UOC

## Fecha

Marzo de 2025
