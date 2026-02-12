# Home-Assistant-Body-Composition-Dashboard
A script for creating an informative dashboard based on data from smart scales (Xiaomi Mi Body Composition Scale 1/2 and others) in Home Assistant.

**Features**

• Interactive notifications: Use the <ha-alert> component for visual status assessment.

• Smart logic: Automatically calculates categories, from "Athletic" to "Dangerous visceral fat levels."

• Flexible customization: Easily adapt to your sensor IDs.

• Standards support: Indicator limits are set according to generally accepted fitness standards and BMI.

**Screenshot**
[soon]

**Installation**

1. Make sure your scale is integrated into Home Assistant (via ESPHome, BLE Monitor, or the official integration).
   
2. Create a new Markdown card on your dashboard.
  
3. Copy the contents of the body_composition.jinja file (or simply paste the code from the repository) into the card's code field.
   
4. Replace the sensor names in the set block with your own:

• sensor.body_score

• sensor.body_fat

• sensor.bmi

• sensor.visceral_fat

• sensor.body_water
