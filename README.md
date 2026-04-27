# Fuel Economy Calculator
[![Github Downloads all Releases](https://img.shields.io/github/downloads/orlandoayeras/fuel-eco-calculator/total)](https://github.com/orlandoayeras/fuel-eco-calculator/releases)
[![Latest Version](https://img.shields.io/github/v/release/orlandoayeras/fuel-eco-calculator)](https://github.com/orlandoayeras/fuel-eco-calculator/releases/latest)
[![License](https://img.shields.io/github/license/orlandoayeras/fuel-eco-calculator)](https://github.com/orlandoayeras/fuel-eco-calculator/blob/main/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/orlandoayeras/fuel-eco-calculator)](https://github.com/orlandoayeras/fuel-eco-calculator/issues)

A lightweight Progressive Web App (PWA) for calculating fuel economy and trip costs for **Gasoline**, **Hybrid EV**, and **Full EV** vehicles. Works in any browser, installable on mobile, and functions offline.

**Live app:** https://orlandoayeras.github.io/fuel-eco-calculator/

---

## Features

- Three vehicle modes: Gasoline, Hybrid EV, Full EV
- Results: Combined Fuel Economy, Cost per km, Cost per 100 km, Total Trip Cost, and full Cost Breakdown
- km / miles unit toggle
- Configurable currency symbol
- Installable as a home screen app (PWA)
- Fully offline after first visit

---

## How to Use

### 1. Choose Your Vehicle Mode

At the top of the app, tap the tab that matches your vehicle:

| Tab | For |
|---|---|
| 🚗 Gasoline | Petrol or diesel vehicles |
| 🔋 Hybrid EV | Plug-in or self-charging hybrids |
| ⚡ Full EV | Pure electric vehicles |

---

### 2. Set Your Units and Currency

In the top-right corner:
- Toggle **KM / MI** to switch between kilometres and miles
- Edit the **currency symbol** (defaults to `$`) to match your local currency (e.g. `₱`, `€`, `£`)

---

### 3. Fill in the Fields

#### 🚗 Gasoline

| Field | What to enter |
|---|---|
| Distance | Total trip distance (km or mi) |
| Fuel Used | Litres of petrol/diesel consumed — from your pump receipt or trip computer |
| Fuel Price | Price per litre at the pump |

#### 🔋 Hybrid EV

| Field | What to enter |
|---|---|
| Distance | Total trip distance |
| Fuel Used | Litres of petrol consumed |
| Fuel Price | Price per litre at the pump |
| Battery Used | kWh drawn from the battery — from your vehicle's energy display or charging app |
| Electricity Price | Cost per kWh from your electricity bill or charging station |

#### ⚡ Full EV

| Field | What to enter |
|---|---|
| Distance | Total trip distance |
| Battery Used | kWh consumed — from your vehicle's energy display or charging app |
| Electricity Price | Cost per kWh |

---

### 4. Tap Calculate

The results dashboard appears below with:

| Result | Meaning |
|---|---|
| **Combined Fuel Economy** | km/L (or MPG) — higher is better |
| **L / 100 km** | Litres per 100 km — lower is better |
| **km / kWh** | Electric efficiency — higher is better |
| **kWh / 100 km** | Energy per 100 km — lower is better |
| **Cost per km** | Total energy cost ÷ distance |
| **Cost per 100 km** | Standard running-cost benchmark for comparing vehicles |
| **Total Trip Cost** | Full energy spend for the trip |
| **Cost Breakdown** | Line-by-line split of fuel and electricity costs |

---

### 5. Tip for Best Accuracy

> Fill your tank from empty → drive your usual route → refill and record the **exact litres pumped** and **odometer distance** travelled. This gives the most accurate real-world figure.

---

## Install as an App

On **mobile**, open the live link in your browser and tap:
- **Android (Chrome):** "Add to Home Screen" banner or menu → Add to Home Screen
- **iPhone (Safari):** Share button → Add to Home Screen

The app installs with an icon and works fully offline.

---

## Deploy Your Own Copy

1. Fork this repository
2. Go to **Settings → Pages**
3. Set source: branch `main`, folder `/ (root)`
4. Your app will be live at `https://<your-username>.github.io/fuel-eco-calculator/`

---

## Files

```
index.html      Main app (single-file PWA)
manifest.json   PWA metadata (name, icons, theme)
sw.js           Service worker (offline caching)
icon.svg        App icon
```
