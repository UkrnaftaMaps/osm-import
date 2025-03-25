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
```xml 
<?xml version='1.0' encoding='UTF-8'?>
<osm version="0.6" generator="JOSM" upload="false">
  <node id="-1" lat="48.12345" lon="37.67890" visible="true">
    <tag k="ref" v="123"/>
    <tag k="addr:full" v="вул. Центральна, 10, м. Краматорськ, Донецька область, Україна, 84300"/>
    <tag k="addr:state" v="Донецька область"/>
    <tag k="addr:ISO3166-2-lvl4" v="UA-14"/>
    <tag k="addr:district" v="Краматорський район"/>
    <tag k="addr:municipality" v="Краматорська міська громада"/>
    <tag k="addr:city" v="Краматорськ"/>
    <tag k="addr:road" v="вул. Центральна"/>
    <tag k="addr:postcode" v="84300"/>
    
    <tag k="fuel:lpg" v="yes"/>
    <tag k="fuel:diesel" v="yes"/>
    <tag k="fuel:octane_92" v="yes"/>
    <tag k="fuel:octane_95" v="yes"/>
    <tag k="fuel:octane_98" v="yes"/>
    <tag k="fuel:adblue" v="yes"/>
    
    <tag k="toilets" v="yes"/>
    <tag k="internet_access" v="wlan"/>
    <tag k="generator" v="yes"/>
    <tag k="amenity" v="fuel"/>
    <tag k="service:coffee" v="yes"/>
    <tag k="shop" v="convenience"/>
    <tag k="parking" v="yes"/>
    <tag k="compressed_air" v="yes"/>
    <tag k="payment:terminal" v="yes"/>
    <tag k="amenity" v="fast_food"/>
    
    <tag k="name" v="АЗС «Укрнафта»"/>
    <tag k="name:en" v="UKRNAFTA Gas Station"/>
    <tag k="name:uk" v="АЗС «Укрнафта»"/>
    
    <tag k="brand" v="UKRNAFTA"/>
    <tag k="brand:uk" v="Укрнафта"/>
    <tag k="brand:en" v="UKRNAFTA"/>
    <tag k="operator" v="ПАТ «Укрнафта»"/>
    
    <tag k="contact:phone" v="+380501234567"/>
    <tag k="contact:email" v="info@ukrnafta.com"/>
    <tag k="contact:website" v="https://www.ukrnafta.com/"/>
    
    <tag k="opening_hours" v="24/7"/>
    
    <tag k="brand:wikidata" v="Q4503721"/>
    <tag k="brand:wikipedia" v="uk:Укрнафта"/>
    
    <tag k="contact:facebook" v="ukrnafta.official"/>
    <tag k="contact:instagram" v="ukrnafta.official"/>
    <tag k="contact:twitter" v="ukrnafta"/>
    <tag k="contact:tiktok" v="ukrnafta.official"/>
    <tag k="contact:youtube" v="ukrnafta"/>
    <tag k="contact:linkedin" v="company/ukrnafta"/>
    
    <tag k="source" v="UKRNAFTA"/>
    <tag k="import" v="yes"/>
  </node>
</osm>
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
