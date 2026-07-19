# HORUS (Healthcare & Operational Reagent Upkeep System)

Anyone who has worked in a laboratory knows how expensive reagents can be. Things like custom RNA primers or high-fidelity polymerases can cost $500 for a tiny vial. In a busy lab, it's easy for students to forget to log when they opened a bottle, or left something in the wrong freezer. When an expensive enzyme spoils or goes past its expiration date, it can ruin weeks of experimental data and squander funds. 

We built **HORUS** as a simple, reliable watchman for lab inventories, replacing manual clipboards with real-time tracking right at the palm of your hands (your tablet maybe).

## What it does
HORUS is a dashboard designed to run on a lab tablet or laptop. It lets people quickly log biological reagents, note their exact storage location (-20°C, -80°C, or 4°C), and keep an eye on their shelf lives. 

The app handles the date math automatically. It calculates the remaining days before a reagent degrades using a linear expiration formula:

$$E_{days} = T_{expiry} - T_{current}$$

If a premium item gets within 7 days of expiring, the dashboard automatically highlights that row in red. This gives the lab team a visual warning so that they don't accidentally use an expired sample in an active experiment.

## Site
Check it out on https://juergenlaturisa.github.io/HORUS/
