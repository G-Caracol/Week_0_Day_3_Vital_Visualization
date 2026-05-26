# Week_0_Day_3_Vital_Visualization
---

# Week_0_Day_3_Visualisation

Day 3 submission for CariSurg MedTech Pathways — data visualisation of the cleaned triage dataset.

**Colab notebook:** [Open in Colab](https://colab.research.google.com/drive/1PUCA495gkXxTPv_sQQylav9LBPYzd5PT?usp=sharing)

## What this notebook does

Loads the Emergency Triage Dataset, applies all cleaning from Days 1-2, then produces six plots:

| # | Plot Type | Variables | Clinical Question |
|---|-----------|-----------|-------------------|
| 1 | Histogram | GCS | Are most patients alert or do many have reduced consciousness? |
| 2 | Histogram | Pulse | How many patients fall outside normal heart rate (60-100 bpm)? |
| 3 | Scatter | SBP vs DBP | Does the blood pressure relationship match what physiology predicts? |
| 4 | Scatter | Age vs Pulse | Does age affect heart rate in this ED population? |
| 5 | Box plots | All vitals | After cleaning, do any vitals still show suspicious spread? |
| 6 | Bar chart | Gender | What is the gender breakdown of patients? |

## Why these plots

Each plot answers a specific clinical question. The reference lines and shaded zones aren't decoration — they mark clinically meaningful thresholds that a triage nurse or doctor would recognise:

- **GCS ≤ 8** is the intubation threshold in many protocols
- **Pulse < 60 or > 100 bpm** flags bradycardia and tachycardia
- **DBP ≈ 0.6 × SBP** is the expected physiological relationship between blood pressure components

Without these anchors, a histogram is just a shape. With them, it becomes a clinical tool.
