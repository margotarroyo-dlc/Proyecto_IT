# ¿Crece la economía sin crecer los residuos?
### Desacoplamiento, eficiencia de reciclaje y cumplimiento de la Directiva UE en el Área Metropolitana de Barcelona (2008–2023)

**Autora:** Marot Arroyo De la Cruz  
**Programa:** Especialización en Data Analytics — IT Academy  
**Fecha:** Febrero 2026  

---

## Descripción

Este proyecto analiza la relación entre crecimiento económico y generación de residuos sólidos en 31 municipios del Área Metropolitana de Barcelona (AMB) entre 2008 y 2023, evaluando si la región cumple con los objetivos de reciclaje de la Directiva europea 2018/851/UE.

**Pregunta de investigación:**  
¿Se ha desacoplado el crecimiento económico de la generación de residuos en el AMB? ¿Existen diferencias entre municipios que permitan diseñar políticas adaptadas a cada realidad?

---

## Hallazgos principales

- **Desacoplamiento relativo confirmado**: el índice de desacoplamiento (DI) fue negativo en 13 de los 15 años analizados, con desacoplamiento genuino desde 2014.
- **Curva de Kuznets Ambiental validada**: punto de inflexión en **16.383 € de PIB per cápita** (R² ajustado = 0,859).
- **El tamaño del hogar, y no la renta, es el factor más asociado a la generación de residuos** (elasticidad = –3,45; p = 0,052).
- **Eficiencia de reciclaje AMB en 2023: 53,2%** — a menos de 2 puntos de la meta del 55% para 2025, pero con una brecha estructural de más de 12 puntos respecto a los líderes europeos.
- **Cinco perfiles municipales** con necesidades de intervención diferenciadas.

---

## Estructura del repositorio

```
├── data/                        # Bases de datos originales
│   ├── bd_características_municipales.xlsx
│   ├── bd_gasto_presupuestario_AMB.xlsx
│   └── bd_gasto_residuos_paises.xlsx
│
├── notebooks/                   # Análisis principal
│   └── 002-analisis_residuos_AMB_fdefinitivo.ipynb
│
├── informe/                     # Informe final
│   └── Informe_definitivo_v6.pdf
│
└── README.md
```

---

## Requisitos y reproducibilidad

### Entorno
- Python 3.10+

### Librerías necesarias
```bash
pip install pandas numpy matplotlib seaborn statsmodels linearmodels scikit-learn
```

### Cómo ejecutar
1. Clona el repositorio:
```bash
git clone https://github.com/[tu-usuario]/[nombre-repo].git
```
2. Coloca los archivos de datos en la carpeta `data/`
3. Abre y ejecuta el notebook en orden:
```bash
jupyter notebook notebooks/002-analisis_residuos_AMB_fdefinitivo.ipynb
```

>  El notebook usa rutas relativas (`Path("data/...)`). Asegúrate de ejecutarlo desde la raíz del repositorio.

---

## Datos y fuentes

| Dataset | Descripción | Fuente |
|---|---|---|
| `bd_características_municipales.xlsx` | Variables socioeconómicas y residuos, 31 municipios, 2008–2023 | AMB, Idescat, INE |
| `bd_gasto_presupuestario_AMB.xlsx` | Gasto del Ayuntamiento de Barcelona en servicios comunitarios | Ajuntament de Barcelona |
| `bd_gasto_residuos_paises.xlsx` | Generación, tratamiento y gasto en residuos por país europeo | Eurostat, FMI |

---

## Visualizaciones generadas

| Figura | Descripción |
|---|---|
| Fig. 1 | Índice de Desacoplamiento (DI) 2008–2023 |
| Fig. 2 | Curva de Kuznets Ambiental (EKC) |
| Fig. 3 | Segmentación estratégica municipal (K-means, k=5) |
| Fig. 4 | Ranking municipal de eficiencia de reciclaje vs. meta UE 55% (2023) |
| Fig. 5 | Distribución de la eficiencia de reciclaje por municipio y año |
| Fig. 6 | Evolución de la tasa de reciclaje por períodos estratégicos (2008–2023) |

---

## Referencias principales

- Grossman, G. M. y Krueger, A. B. (1995). *Economic growth and the environment*. The Quarterly Journal of Economics, 110(2), 353–377.
- Stern, D. I. (2004). *The rise and fall of the environmental Kuznets curve*. World Development, 32(8), 1419–1439.
- Parlamento Europeo. (2018). *Directiva 2018/851/UE*. Diario Oficial de la Unión Europea.
- Wu, H. y Li, M. (2025). *Testing the existence of waste Kuznets curve hypothesis in 45 emerging economies*. Journal of Environmental Management, 373.

---

## Licencia

Este proyecto se comparte únicamnete con fines académicos bajo licencia [MIT](https://opensource.org/licenses/MIT).
