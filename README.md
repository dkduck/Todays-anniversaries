# 🎉 TODAY – Dynamic Day‑Info Card for Home Assistant

A clean, elegant, fully automated *“What day is it today?”* card for Home Assistant, built using **custom:button-card** and pure JavaScript logic.  
The card displays a daily icon, title, and subtitle — including holidays, flag days, UN days, unofficial theme days, and personal events.

---

## ✨ Features

- **Automatic date detection**
- **100+ Danish holidays, theme days, and cultural dates**
- **Support for personal events** (birthdays, anniversaries)
- **Beautiful layout** with icon, headline, and description
- **Fallback message** when no special day exists
- **Transparent background** and pixel‑perfect Home Assistant styling
- **No dependencies** beyond `custom:button-card`

---

## 📦 Installation

### Requirements

- Home Assistant  
- HACS  
- `custom:button-card` installed  

### Adding the Card

1. Open your Home Assistant dashboard  
2. Add a **Manual Card**  
3. Paste the YAML from the `/card.yaml` file in this repository  

The card will automatically detect today’s date and display the correct event.

---

## 🧠 How It Works

The card uses a JavaScript dictionary containing all special days in the format:


The current date is detected automatically, and the matching entry is shown.  
If no entry exists, a fallback message is displayed:

> *“Just an ordinary day”*

---

## 🛠️ Customization

You can easily:

- Add new special days  
- Modify icons, titles, or descriptions  
- Change colors to match your dashboard theme  
- Replace fallback text with your own wording  

All customization happens inside the `dage` object in the YAML file.

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| **card.yaml** | The full card logic and styling |
| **README.md** | Project documentation |
| **assets/** | Screenshots and images |

---

## 🚀 Future Ideas

- Seasonal color themes  
- API‑based flag day detection  
- Calendar sensor integration  
- Animated icons on special days  

---

## ❤️ Contributing

Pull requests are welcome — especially new special days, styling improvements, or optimizations.

---

## 📜 License

MIT License — free to use, modify, and include in your own dashboards.

