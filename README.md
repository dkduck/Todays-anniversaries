🎉 TODAY – Dynamic Day‑Info Card for Home Assistant
A clean, elegant, fully automated “What day is it today?” card for Home Assistant, built using custom:button-card and pure JavaScript logic.
The card displays a daily icon, title, and subtitle — including holidays, flag days, UN days, unofficial theme days, and your own personal dates.

✨ Features
Automatic date detection

100+ Danish holidays, theme days, UN days, and personal events

Custom personal dates (e.g., birthdays)

Beautiful layout with icon, headline, and description

Fallback message when no special day exists

Transparent background and pixel‑perfect Home Assistant styling

No dependencies beyond custom:button-card

📦 Installation
Add the card to your Home Assistant dashboard using YAML or a Manual Card.

Requirements
Home Assistant

HACS

custom:button-card installed

Add the card
Insert the YAML code from /card.yaml into your dashboard.

🧠 How It Works
The card contains a large JavaScript object with all special days in the format:

js
"22-09": { ikon: "🎁", tekst: "Erik Birthday", sub: "Birthday" }
The current date is detected automatically:

js
const md = String(nu.getDate()).padStart(2, '0') + '-' + String(nu.getMonth() + 1).padStart(2, '0');
If the date exists in the list → show the matching day.
If not → show the fallback message “Just an ordinary day”.

🖼️ Example Preview
How the card appears inside Home Assistant:





📁 Project Structure
File	Description
card.yaml	The full card including all day‑logic
README.md	Documentation and project overview
assets/	Screenshots and graphics (optional)


🛠️ Customization
Add your own special days easily:

js
"17-07": { ikon: "🍹", tekst: "Gin Hass Day – Christina/Erik", sub: "Family Day" }
Or change the fallback:

js
tekst: "Nothing special today"
🚀 Future Ideas
Automatic flag‑day detection via API

Seasonal color themes

Calendar sensor integration

Animations on special days

❤️ Contributing
Pull requests are welcome — especially new special days, styling improvements, or JavaScript optimizations.

📜 License
MIT License — free to use in your dashboards.
