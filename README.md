# MR & TR Quantification Calculator

A comprehensive, single-page echocardiographic calculator for quantifying **Mitral Regurgitation (MR)** and **Tricuspid Regurgitation (TR)** severity using multiple validated methods.

🔗 **[Live Demo →](https://your-username.github.io/mr-tr-calculator/)**

---

## Features

### Methods Supported

#### Mitral Regurgitation (MR)
| Method | Outputs |
|--------|---------|
| **PISA / EROA** | PISA flow, EROA (cm²), Regurgitant Volume (mL) |
| **Continuity Equation** | LVOT SV, MV SV, RVol (mL), Regurgitant Fraction (%) |
| **Quantitative Doppler** | LVOT vs PV comparison, RVol, RF, Cardiac Output |

#### Tricuspid Regurgitation (TR)
| Method | Outputs |
|--------|---------|
| **PISA / EROA** | PISA flow, EROA (cm²), Regurgitant Volume (mL) |
| **Continuity Equation** | TV SV, PV SV, RVol, RF |
| **Quantitative Doppler** | TV vs RVOT comparison, RVol, RF, Cardiac Output |
| **RVSP Estimator** | Bernoulli equation with RAP adjustment |

### Severity Grading
- Real-time color-coded severity pills (Mild / Moderate / Severe / Torrential)
- Based on **2017 AHA/ACC** and **2021 ESC/EACTS** Valvular Heart Disease Guidelines
- Comprehensive reference tables with intervention thresholds

---

## Formulas

### PISA / EROA
```
PISA Flow (mL/s) = 2π × r² × Va
EROA (cm²)       = Flow / Vmax
RVol (mL)        = EROA × VTI
```

### Continuity Equation (MR example)
```
LVOT SV (mL) = π × (LVOT d / 2)² × LVOT VTI
MV SV (mL)   = π × (MV d / 2)² × MV VTI
RVol (mL)    = MV SV − LVOT SV
RF (%)       = RVol / MV SV × 100
```

### Quantitative Doppler (Left Heart)
```
LVOT SV (mL) = π × (LVOT d / 2)² × LVOT VTI
PV SV (mL)   = π × (PV d / 2)² × PV VTI
RVol (mL)    = LVOT SV − PV SV
RF (%)       = RVol / LVOT SV × 100
```

### RVSP (Bernoulli)
```
RVSP (mmHg)  = 4 × TR Vmax² + RAP
```

---

## Severity Cutoffs

### MR (AHA/ACC 2017)
| Parameter | Mild | Moderate | Severe |
|-----------|------|----------|--------|
| EROA (cm²) | < 0.20 | 0.20–0.39 | ≥ 0.40 |
| RVol (mL) | < 30 | 30–59 | ≥ 60 |
| RF (%) | < 30 | 30–49 | ≥ 50 |

### TR (ESC 2021)
| Parameter | Mild | Moderate | Severe | Torrential |
|-----------|------|----------|--------|------------|
| EROA (cm²) | < 0.20 | 0.20–0.39 | 0.40–0.59 | ≥ 0.60 |
| RVol (mL) | < 30 | 30–44 | 45–74 | ≥ 75 |
| RF (%) | < 30 | 30–49 | ≥ 50 | — |

---

## Usage

No installation required. Simply open `index.html` in any modern browser.

**Or deploy to GitHub Pages:**
1. Fork this repository
2. Go to Settings → Pages
3. Set source to `main` branch, root directory
4. Visit `https://your-username.github.io/mr-tr-calculator/`

---

## Clinical Disclaimer

> This calculator is intended as an **educational and computational aid** for trained echocardiographers and cardiologists. Results must be interpreted in conjunction with complete clinical and echocardiographic evaluation. Grading of valvular regurgitation requires integration of multiple parameters. Always follow current institutional and professional society guidelines.
>
> **Not for direct patient management decisions without physician oversight.**

---

## References

1. Nishimura RA, et al. *2017 AHA/ACC Focused Update of the 2014 AHA/ACC Guideline for the Management of Patients With Valvular Heart Disease.* JACC. 2017.
2. Vahanian A, et al. *2021 ESC/EACTS Guidelines for the management of valvular heart disease.* Eur Heart J. 2022.
3. Zoghbi WA, et al. *Recommendations for Evaluation of the Severity of Native Valvular Regurgitation with Two-Dimensional and Doppler Echocardiography.* JASE. 2003.
4. Lang RM, et al. *Recommendations for Cardiac Chamber Quantification by Echocardiography in Adults.* JASE. 2015.

---

## License

MIT License — free to use for educational purposes.
