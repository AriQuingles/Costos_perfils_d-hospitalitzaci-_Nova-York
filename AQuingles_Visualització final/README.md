# Qui concentra més cost hospitalari a Nova York i per què?

Projecte final de visualització de dades basat en el conjunt **SPARCS – Hospital Inpatient Discharges (de-identified), 2024**.

## Resum del projecte
Aquest projecte analitza **qui concentra més cost hospitalari a Nova York i per què**, combinant una perspectiva:
- **clínica**
- **demogràfica**
- **econòmica**

La visualització final s'ha construït com una **història interactiva a Flourish**, i parteix d'un procés previ de **preparació, neteja, selecció i agregació de dades a Jupyter Notebook**.

## Tipus de dades
**Clíniques, demogràfiques i econòmiques**

## Font de dades
**New York State Department of Health**, portal **Health Data NY**

- Dataset: **SPARCS – Hospital Inpatient Discharges (de-identified), 2024**
- Enllaç del dataset (2024):  
  https://health.data.ny.gov/Health/Hospital-Inpatient-Discharges-SPARCS-De-Identified/sf4k-39ay

## Abast
- **Àmbit geogràfic:** Nova York
- **Any analitzat:** 2024
- **Volum aproximat:** més de **2,19 milions d’hospitalitzacions inpatient** en un sol any

## Objectiu
Explorar i comunicar quins factors s’associen a una major càrrega econòmica hospitalària, posant el focus en:
- perfil del pacient
- tipus d’ingrés
- severitat clínica
- diagnòstic

## Preguntes principals
1. El cost és igual per a tots els perfils de pacient?
2. Quins tipus d’ingrés són més cars i més complexos?
3. Com canvien el cost i l’estada a mesura que augmenta la severitat clínica?
4. Quins diagnòstics pesen més sobre el sistema hospitalari?

## Eines utilitzades
- **Anàlisi de dades:** Jupyter Notebook
- **Visualització:** Flourish
- **Edició del vídeo:** DaVinci Resolve

## Procés de treball
El projecte s'ha desenvolupat en aquestes fases:

1. **Descàrrega** del dataset SPARCS 2024
2. **Inspecció i neteja** de variables rellevants
3. **Conversió** de formats i creació de mètriques derivades
4. **Agregació** del dataset en fitxers resumits en CSV
5. **Construcció** de la narrativa visual a Flourish
6. **Presentació** en vídeo del procés, la lògica analítica i la visualització final

## Fitxers del repositori

### Codi
- `SPARCS_PR2_preparacio_dades_corregit.ipynb`  
  Notebook principal de preparació de dades i creació dels CSV finals.

### Documentació
- `README.md`  
  Descripció del projecte i instruccions d'ús.
- `LICENSE`  
  Llicència MIT.
- `requirements.txt`  
  Dependències mínimes per executar el notebook.
- `docs/Part_I_seleccio_conjunt_dades.pdf` *(opcional però recomanat)*  
  Document de la Part I del projecte.

### Fitxers de dades derivats
Aquest projecte genera o utilitza fitxers CSV resumits, com ara:
- `overview_kpis.csv`
- `cost_by_age_gender.csv`
- `cost_by_age_gender_clean.csv`
- `cost_by_admission.csv`
- `cost_by_admission_clean.csv`
- `severity_vs_cost.csv`
- `diagnosis_or_area.csv`
- fitxers derivats addicionals per a Flourish segons la configuració final de la història

> **Important:** Per privacitat i mida del fitxer, no és necessari incloure el dataset complet SPARCS 2024 al repositori si és massa pesat. N'hi ha prou amb incloure el notebook, els fitxers resumits que has generat i l'enllaç oficial a la font.

## Estructura recomanada del repositori

```text
project-root/
│
├── README.md
├── LICENSE
├── requirements.txt
├── SPARCS_PR2_preparacio_dades_corregit.ipynb
│
├── data/
│   ├── overview_kpis.csv
│   ├── cost_by_age_gender.csv
│   ├── cost_by_age_gender_clean.csv
│   ├── cost_by_admission.csv
│   ├── cost_by_admission_clean.csv
│   ├── severity_vs_cost.csv
│   ├── diagnosis_or_area.csv
│   └── altres_csv_derivats.csv
│
└── docs/
    └── Part_I_seleccio_conjunt_dades.pdf
```

## Com executar el notebook

### 1. Clonar el repositori
```bash
git clone https://github.com/EL_TEU_USUARI/EL_TEU_REPOSITORI.git
cd EL_TEU_REPOSITORI
```

### 2. Crear entorn i instal·lar dependències
```bash
pip install -r requirements.txt
```

### 3. Obrir Jupyter Notebook
```bash
jupyter notebook
```

### 4. Executar
Obre:
```text
SPARCS_PR2_preparacio_dades_corregit.ipynb
```
i executa les cel·les per generar els CSV resumits necessaris per a la visualització.

## Publicació de la visualització
La visualització final està publicada a **Flourish** i és accessible públicament sense registre.

- **Enllaç a la visualització:** `AFEGIR_ENLLAÇ_FLOURISH`
- **Enllaç al vídeo:** `AFEGIR_ENLLAÇ_VIDEO`
- **Enllaç al repositori GitHub:** `AFEGIR_ENLLAÇ_REPOSITORI`

## Entrega recomanada
Per a l'entrega final, comprova que:
- el repositori GitHub és **públic**
- la visualització de Flourish és **pública**
- el vídeo és accessible
- el notebook i els fitxers resumits estan pujats
- hi ha una **llicència de codi obert**
- el README explica clarament:
  - d'on venen les dades
  - quin tipus de dades són
  - com s'han treballat
  - quines eines s'han utilitzat
  - on es pot veure la visualització final

## Consideracions ètiques
Tot i tractar-se d’un dataset **desidentificat**, continua essent informació sanitària sensible. Per això:
- no s’han fet interpretacions causals no justificades
- s’ha evitat qualsevol lectura estigmatitzadora
- la visualització se centra en patrons agregats i no en casos individuals

## Autoría
**Ariadna Quingles Lamarca**  
Projecte final de l’assignatura de Visualització de dades
