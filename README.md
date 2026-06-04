
<h1 align="center">KORIA — GabèsEye</h1>

<p align="center">
  <b>AI-powered environmental monitoring platform</b> — H12 INNOVATION 3.0
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat&logo=dart&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Airbyte-615EFF?style=flat&logo=airbyte&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" />
</p>

---

## Overview

**GabèsEye** is a cross-platform environmental surveillance application developed during the **H12 INNOVATION 3.0** national hackathon. It combines satellite imagery analysis, real-time sensor data, and AI-powered forecasting to deliver actionable environmental intelligence.

The system monitors soil contamination, water turbidity, and air quality — giving field teams and researchers a real-time dashboard for environmental decision-making.

---

## Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                    GABÈSEYE SYSTEM                                 │
│                                                                   │
│  Satellite Imagery ──→ PyTorch Segmentation Models                │
│       (multispectral)      ├── Soil contamination classification  │
│                            └── Water turbidity detection          │
│                                                                   │
│  Field Sensors ────────→ Airbyte Sync ──→ Central Database        │
│       (IoT devices)           └── No manual data wrangling        │
│                                                                   │
│  Central DB ───────────→ scikit-learn Time-Series Models          │
│                              ├── Contamination trend forecasting  │
│                              └── Air quality prediction           │
│                                                                   │
│  API Layer (FastAPI) ──→ Flutter Cross-Platform App              │
│                              ├── Interactive maps (flutter_map)   │
│                              ├── Real-time charts (fl_chart)      │
│                              ├── Multilingual chatbot interface   │
│                              └── Biometric auth (local_auth)      │
└─────────────────────────────────────────────────────────────────┘
```

---

## Features

| Feature | Details |
|---------|---------|
| 🛰 **Satellite Segmentation** | PyTorch models on multispectral imagery classify soil contamination and detect water turbidity |
| 🌊 **Water Quality** | Real-time turbidity monitoring with trend forecasting |
| 🌬 **Air Quality** | Predictive models for contamination levels and air quality index |
| 📊 **Interactive Dashboards** | Charts and maps powered by `fl_chart` and `flutter_map` |
| 🗺 **Geospatial Mapping** | OpenStreetMap integration with `latlong2` for field data visualization |
| 🤖 **AI Chatbot** | Multilingual natural language interface for querying environmental data |
| 🔐 **Secure Access** | Biometric authentication with `local_auth` |
| 🌐 **Multi-language** | Full internationalization support via `intl` and `flutter_localizations` |

---

## Tech Stack

### Frontend (This Repo)

| Layer | Technology |
|-------|-----------|
| **Framework** | Flutter 3.x |
| **Language** | Dart 3.x |
| **State Management** | Provider |
| **Maps** | flutter_map + latlong2 |
| **Charts** | fl_chart |
| **Icons** | Cupertino Icons |
| **Typography** | Google Fonts |
| **Local Storage** | Shared Preferences |
| **Auth** | Local Authentication (biometrics) |
| **HTTP Client** | http package |
| **Animations** | Shimmer |

### Backend / ML (Separate)

| Component | Technology |
|-----------|-----------|
| **Satellite Segmentation** | PyTorch |
| **Time-Series Forecasting** | scikit-learn |
| **Data Integration** | Airbyte |
| **API** | FastAPI |
| **Database** | PostgreSQL |

---

## Getting Started

### Prerequisites

- Flutter SDK ^3.10.8
- Dart SDK ^3.10.8
- An API endpoint running the FastAPI backend

### Run the App

```bash
# Clone the repository
git clone https://github.com/adriansalvadorekomo/KORIA.git
cd KORIA

# Get dependencies
flutter pub get

# Run the app
flutter run
```

The app supports **Android**, **iOS**, **Web**, **Linux**, **macOS**, and **Windows**.

---

## Project Structure

```
lib/
├── data/         # Data layer (models, repositories)
├── l10n/         # Localization files
├── models/       # Data models
├── providers/    # State management (Provider)
├── screens/      # UI screens
├── services/     # API services and business logic
├── theme/        # App theming
└── main.dart     # Entry point
```

---

## Hackathon Context

Built for **H12 INNOVATION 3.0** — a national innovation hackathon focused on environmental technology. The project was designed to address real environmental monitoring challenges in the Gabès region, combining satellite remote sensing with ground-level IoT sensor data for comprehensive environmental surveillance.

---

## Related

| Resource | Link |
|----------|------|
| 📄 CV (Multi-Language) | [Download PDFs](https://github.com/adriansalvadorekomo/adriansalvadorekomo/tree/main/cv) |
| 🏗 Data Engineering Portfolio | [Profile](https://github.com/adriansalvadorekomo) |
| 📊 Event Analytics Platform | [EventZilla BI](https://github.com/adriansalvadorekomo/Esprit-PABI-4ERPBI6-2526-EventZella) |
| 🗄 Smart-ERP DataOps | [ERP System](https://github.com/adriansalvadorekomo/smart-erp-dataopts) |

---

<p align="center">
  <sub>H12 INNOVATION 3.0 · Environmental Intelligence Through AI & Data Engineering</sub>
</p>
