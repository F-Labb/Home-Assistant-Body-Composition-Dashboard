# 📊 Home Assistant Body Composition Dashboard

A customizable Markdown-based dashboard for Home Assistant that visualizes data from smart scales (Xiaomi Mi Body Composition Scale 1/2 and others). 

This project provides high-visibility alerts and motivational feedback based on your body metrics.

## ✨ Features
- **Dynamic Alerts:** Uses `<ha-alert>` components that change color based on your results.
- **Gender-Specific Logic:** Separate templates for Male and Female users with adjusted physiological norms (Fat %, Water %).
- **Easy Setup:** All sensor configurations are moved to the top of the script for quick replacement.
- **Multilingual:** Supports both English and Russian languages.

## 📸 Preview

![Dashboard Example](https://github.com/F-Labb/Home-Assistant-Body-Composition-Dashboard/blob/main/preview.jpeg)

## 🚀 Installation

1. Create a new **Markdown Card** on your Home Assistant dashboard.
2. Choose the version you need from this repository:
   - `male_en.jinja` / `male_ru.jinja`
   - `female_en.jinja` / `female_ru.jinja`
3. Copy the code and paste it into the card.
4. **Important:** Update the configuration block at the top of the script with your actual entity IDs:

```jinja
{# --- CONFIGURATION: CHANGE YOUR SENSOR IDS HERE --- #}
{% set score_sensor = 'sensor.YOUR_body_score' %}
{% set fat_sensor = 'sensor.YOUR_body_fat' %}
{% set bmi_sensor = 'sensor.YOUR_bmi' %}
{% set visceral_sensor = 'sensor.YOUR_visceral_fat' %}
{% set water_sensor = 'sensor.YOUR_water' %}
{# -------------------------------------------------- #}
```
## 📈 Metric Standards

The dashboard tracks and evaluates:
• Body Score: Overall health rating.

• Body Fat: Categorized from Athletic to Obesity.

• BMI: Standard WHO classifications.

• Visceral Fat: Internal fat levels and health risks.

• Hydration: Optimal water percentage.
