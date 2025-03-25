---

# 🗺️ UKRNAFTA Gas Stations Import

This repository contains tools, data, and documentation for importing the official gas station dataset from **PJSC "Ukrnafta"** into **OpenStreetMap**.

## 📌 Summary
- **Data Provider:** PJSC "Ukrnafta"
- **Importer:** 4Service UA (Vitaly Vlasyuk – v.vlasyuk@4service-group.com)
- **License:** Open Database License (ODbL)
- **Objects:** ~600 fuel stations
- **Coverage:** All of Ukraine
- **Import Type:** One-time, semi-automated with validation
- **Wiki Page:** [Import/UKRNAFTA on OSM Wiki](https://wiki.openstreetmap.org/wiki/Import/UKRNAFTA)

---

## 📂 Source Data

- 📄 [CSV Dataset](https://raw.githubusercontent.com/UkrnaftaMaps/osm-import/refs/heads/main/ukrnafta_gas_station.csv)  
- 📑 [License Confirmation (ODbL)](https://github.com/UkrnaftaMaps/osm-import/blob/main/docs/ukrnafta_license_confirmation.pdf)

The dataset includes:
- Coordinates (latitude, longitude)
- Address components
- Fuel types: diesel, LPG, octane_92/95/98, adblue
- Services: toilets, wifi, shop, parking, charging station, fast food
- Contacts: phone, email, website, social media
- Brand and operator tags

---

## 🧩 Tag Mapping

Key fields from the dataset are automatically converted into valid OSM tags.  
See the full [Wiki Mapping Table](https://wiki.openstreetmap.org/wiki/Import/UKRNAFTA#Data_Mapping) for details.

Example:
```yaml
ref: "0123"
lat/lon: node location
addr:full: "Kharkivska oblast, Sumy city, ... "
fuel:octane_95: "yes"
internet_access: "wlan"
brand: "UKRNAFTA"
operator: "ПАТ «Укрнафта»"
```

---

## ⚙️ Tools & Workflow

- 🔄 Data preparation in Google Colab
- 🧪 Validation with JOSM + Conflation plugin
- 🚀 Staged upload region-by-region
- ✅ Community review via mailing list & Telegram

---

## 📬 Contacts

| Role              | Contact                              |
|-------------------|--------------------------------------|
| Import Lead       | Vitaly Vlasyuk — v.vlasyuk@4service-group.com |
| OSM Community     | [imports@openstreetmap.org](https://lists.openstreetmap.org/listinfo/imports) |
| Wiki Page         | [Import/UKRNAFTA](https://wiki.openstreetmap.org/wiki/Import/UKRNAFTA)

---

## 🤝 Contributing

Want to help? Open an issue or contact us!  
Pull requests and reviews are welcome — this is an open import for the benefit of the OSM ecosystem.

---
