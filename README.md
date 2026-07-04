##HORUS (Healthcare & Operational Reagent Upkeep System)##

## Inspiration
Anyone who has worked in a laboratory knows how expensive reagents can be. Things like custom RNA primers or high-fidelity polymerases can cost $500 for a tiny vial. In a busy lab, it's easy for students to forget to log when they opened a bottle, or left something in the wrong freezer. When an expensive enzyme spoils or goes past its expiration date, it can ruin weeks of experimental data and squander funds. 

We built **HORUS (Healthcare & Operational Reagent Upkeep System)** as a simple, reliable watchman for lab inventories, replacing manual clipboards with real-time tracking right at the palm of your hands (your tablet maybe).

## What it does
HORUS is a dashboard designed to run on a lab tablet or laptop. It lets people quickly log biological reagents, note their exact storage location (-20°C, -80°C, or 4°C), and keep an eye on their shelf lives. 

The app handles the date math automatically. It calculates the remaining days before a reagent degrades using a linear expiration formula:

$$E_{days} = T_{expiry} - T_{current}$$

If a premium item gets within 7 days of expiring, the dashboard automatically highlights that row in red. This gives the lab team a visual warning so that they don't accidentally use an expired sample in an active experiment.

## How we built it
We wrote the core logic with JavaScript to handle the dataset sorting and math. For the layout, we used Tailwind CSS to build a cool UI that is easy to read. The entire project is placed in a repository on GitHub and deployed live on the web using GitHub Pages.

## Challenges we ran into
Since we decided to build this without a massive database infrastructure, managing all the dates and state changes purely through browser-side JavaScript was a bit tricky at first. Getting the date subtraction logic to update without causing weird visual glitches in the data table took some trial and error. We also fought the urge to add a lot of features so we could focus on making the main idea feel more solid.

## Accomplishments that we're proud of
We are proud of creating a fully functioning tool to a specific, real-world problem in scientific research. The interface feels easy to navigate and the logic functions exactly how we want it to, which is a big win.

## What we learned
We both learned very different things from this. Juergen learned a great lesson in bridging between life sciences and programming, and Clarissa learned some simple browser logic and how to optimize UI layouts.

## What's next for HORUS
We would love to make something like mobile barcode or QR code scanning, so researchers can just use a phone camera to instantly check a vial into the system. We are also looking into adding simple email or text alerts so lab managers can get a notification before an expensive chemical goes to waste.
