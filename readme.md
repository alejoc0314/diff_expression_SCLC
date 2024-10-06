# Análisis de Expresión Génica y Redes Booleanas en Cáncer de Colon

Este proyecto tiene como objetivo realizar un análisis exhaustivo de los genes expresados diferencialmente en cáncer de colon mediante el uso de herramientas avanzadas de bioinformática. Incluye el uso de algoritmos de análisis de expresión génica diferencial y la simulación de redes booleanas para modelar la interacción entre genes. Además, se emplean bibliotecas especializadas para el análisis de enriquecimiento funcional y la evaluación de redes de interacción proteica.

## Tabla de Contenidos
- [Descripción General](#descripción-general)
- [Importancia de DESeq2](#importancia-de-deseq2)
- [Redes Booleanas](#redes-booleanas)
- [Enrichr para Análisis de Enriquecimiento](#enrichr-para-análisis-de-enriquecimiento)
- [STRING para Redes de Interacción Proteica](#string-para-redes-de-interacción-proteica)
- [GSCA para el Análisis de Caminos Genéticos](#gsca-para-el-análisis-de-caminos-genéticos)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)

## Descripción General

Este proyecto combina varias metodologías y herramientas bioinformáticas con el objetivo de identificar genes clave en el desarrollo y progresión del cáncer de colon. A través del análisis de expresión génica diferencial y la simulación de redes booleanas, buscamos modelar cómo las alteraciones en la expresión génica pueden influir en la enfermedad. Además, se realiza un análisis de enriquecimiento funcional utilizando Enrichr, así como la exploración de redes de interacción proteica con STRING y el análisis de rutas genéticas con GSCA.

## Importancia de DESeq2

**DESeq2** es una de las herramientas más robustas para el análisis de expresión génica diferencial. En este proyecto, DESeq2 se emplea para identificar genes que están significativamente sobre-expresados o sub-expresados en muestras de cáncer de colon en comparación con muestras normales. La importancia de DESeq2 radica en su capacidad para:

- Manejar datos de RNA-seq de manera eficiente.
- Ajustar los valores de p mediante métodos estadísticos robustos como Benjamini-Hochberg (BH) y Holm para controlar la tasa de falsos positivos.
- Identificar genes candidatos que podrían estar implicados en la progresión de la enfermedad o ser posibles biomarcadores.

## Redes Booleanas

Para entender la dinámica de interacción entre los genes identificados, se emplea el modelado de **Redes Booleanas**. Estas redes permiten simular los efectos de la activación o inhibición de genes en función de sus interacciones. En el contexto del cáncer de colon, estas redes nos permiten predecir cómo diferentes combinaciones de activaciones y desactivaciones génicas afectan el sistema en su totalidad.

El enfoque booleano es particularmente útil para estudiar:
- **Estados estables** de expresión génica.
- **Atractores** que representan posibles estados patológicos del sistema.
- Los efectos de mutaciones o alteraciones en genes clave.

## Enrichr para Análisis de Enriquecimiento

**Enrichr** es una biblioteca en línea que facilita el análisis de enriquecimiento funcional. Se utiliza para identificar qué procesos biológicos, rutas metabólicas, o categorías funcionales están sobre-representadas en los genes expresados diferencialmente. Enrichr combina diversas bases de datos, permitiendo:

- Análisis de enriquecimiento basado en ontologías como **GO** (Gene Ontology) y **KEGG**.
- Visualización de los resultados en términos de **procesos biológicos**, **funciones moleculares** y **componentes celulares**.
- Identificación de **vías metabólicas** y otros procesos que podrían estar afectados por los genes en estudio.

## STRING para Redes de Interacción Proteica

El uso de **STRING** en este proyecto es clave para construir redes de interacción proteica, basadas en los genes expresados diferencialmente. STRING proporciona una plataforma integral para analizar y visualizar las interacciones proteína-proteína, permitiendo:

- Explorar conexiones conocidas y predecir nuevas interacciones basadas en evidencia experimental y de texto.
- Construir redes de interacción que destacan las proteínas más conectadas, lo cual es importante para entender las funciones coordinadas dentro de la célula.
- Priorizar genes o proteínas para estudios posteriores en función de su conectividad dentro de la red.

## GSCA para el Análisis de Caminos Genéticos

La **Gene Set Cancer Analysis (GSCA)** es una herramienta utilizada en este proyecto para analizar conjuntos de genes asociados con rutas genéticas y evaluar su impacto en la progresión del cáncer. GSCA permite realizar análisis multivariados para:

- Estudiar la coexpresión de genes dentro de conjuntos definidos, como rutas de señalización o módulos funcionales.
- Evaluar cómo las alteraciones en múltiples genes pueden afectar las vías involucradas en el cáncer de colon.
- Determinar la relevancia biológica de las interacciones entre los genes expresados diferencialmente.

## Requisitos

Para ejecutar este proyecto, necesitarás los siguientes paquetes y bibliotecas:

- R (versión 4.0 o superior)
  - DESeq2
  - EnhancedVolcano
- Python 3.x
  - Biblioteca STRING para la interacción de proteínas

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/alejoc0314/diff_expression_SCLC.git

2. Instala los paquetes requeridos en R:
    ```bash
    install.packages("DESeq2")
    install.packages("EnhancedVolcano")



