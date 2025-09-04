# Granulometría_45

**Granulometría_45** es una aplicación de ciencia de datos con python, para escritorio y diseñada para realizar un análisis granulométrico de mezclas asfálticas bajo la especificación **AASHTO M323** utilizando la gráfica de potencia 0.45 de la **FHWA**. La herramienta está orientada a profesionales y técnicos en ingeniería de pavimentos y tiene como objetivo optimizar el diseño de mezclas asfálticas mediante un análisis interactivo.

Link para descarga: https://github.com/germancruzram/GRANULOMETRIA_45/releases/download/GRANULOMETRIA_45__v2.0/GRANULOMETRIA_45__v2_20.exe

## Características principales

### 🛠️ **Herramientas de Análisis**

- **Análisis Interactivo**: Permite ingresar datos de diseño y visualizar la curva granulométrica al instante.
- **Optimización de Mezclas**: Determina las proporciones óptimas de hasta 5 agregados para cumplir con las especificaciones **SUPERPAVE**.
- **Generación de Reportes**: Exporta informes completos en formato PDF con los datos del proyecto, la tabla granulométrica y la gráfica final.

### 📈 **Visualización de Resultados**

- Visualiza la curva granulométrica junto con las **líneas de máxima densidad** y **bandas de especificación**.
- Muestra las **marcas Bailey** y permite ajustar las proporciones de los agregados en función de los resultados obtenidos.

### 🗂️ **Gestión de Proyectos** (requiere licencia)

- **Guardar y cargar proyectos**: Facilita la organización de diferentes proyectos y su análisis histórico.
- **Configuración personalizable**: Permite ajustar las especificaciones de granulometría y optimización.

## 📊 **Gráfico de Estructura de la Aplicación**

```mermaid
graph TD

    6["User<br>External Actor"]

    subgraph 2["Licensing and Security System<br>Python"]
        17["License Verification Module<br>Python"]
        18["ID Generator<br>Python"]
        19["Public Key Storage<br>PEM"]
        %% Edges at this level (grouped by source)
        17["License Verification Module<br>Python"] -->|Uses| 19["Public Key Storage<br>PEM"]
    end

    subgraph 3["File Operations and Data Management System<br>Python"]
        14["File Operations Handler<br>Python"]
        15["Report Generator<br>Python"]
        16["Project Data Management<br>JSON"]
        %% Edges at this level (grouped by source)
        15["Report Generator<br>Python"] -->|Uses| 14["File Operations Handler<br>Python"]
        16["Project Data Management<br>JSON"] -->|Loaded/Saved via| 14["File Operations Handler<br>Python"]
    end

    subgraph 4["User Interface (UI) System<br>Python"]
        11["Main Application Interface<br>Python"]
        12["UI Components Library<br>Python"]
        13["UI Tables Module<br>Python"]
        %% Edges at this level (grouped by source)
        11["Main Application Interface<br>Python"] -->|Integrates| 12["UI Components Library<br>Python"]
        11["Main Application Interface<br>Python"] -->|Integrates| 13["UI Tables Module<br>Python"]
    end

    subgraph 5["Core Granulometry and Optimization System<br>Python"]
        10["Bailey Method Optimizer<br>Python"]
        7["Bailey Method Implementation<br>Python"]
        8["Optimization Algorithms<br>Python"]
        9["Advanced Optimizer<br>Python"]
        %% Edges at this level (grouped by source)
        10["Bailey Method Optimizer<br>Python"] -->|Interacts with| 7["Bailey Method Implementation<br>Python"]
        10["Bailey Method Optimizer<br>Python"] -->|Uses| 8["Optimization Algorithms<br>Python"]
        9["Advanced Optimizer<br>Python"] -->|Builds upon| 8["Optimization Algorithms<br>Python"]
    end

    %% Edges at this level (grouped by source)
    11["Main Application Interface<br>Python"] -->|Handles data via| 3["File Operations and Data Management System<br>Python"]
    11["Main Application Interface<br>Python"] -->|Performs calculations via| 5["Core Granulometry and Optimization System<br>Python"]
    11["Main Application Interface<br>Python"] -->|Verifies license via| 17["License Verification Module<br>Python"]
    6["User<br>External Actor"] -->|Interacts with| 11["Main Application Interface<br>Python"]
    5["Core Granulometry and Optimization System<br>Python"] -->|Provides data to| 15["Report Generator<br>Python"]


```


## 🤝**Contribuciones y recomendaciones**

Son bienvenidas. En el perfil se encuentra mi contacto.

## 👨‍💻**Autor**

German Ahmed Cruz Ramírez  
[LinkedIn](https://www.linkedin.com/in/german-cruz-ram-in24/)
