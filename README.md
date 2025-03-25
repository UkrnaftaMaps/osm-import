# UKRNAFTA OSM Import Project

This repository contains official data provided by PJSC "Ukrnafta" for the mass import of all their gas station locations across Ukraine into OpenStreetMap (OSM).

## Dataset

- **Source:** PJSC "Ukrnafta"
- **License:** Open Database License (ODbL)
- **Format:** CSV
- **Fields:** id, name, latitude, longitude, address, opening_hours, contact_phone, fuel_types, services

## Files

- `data/ukrnafta_gas_stations.csv` — raw data provided by the company
- `scripts/convert_to_osm.py` — converts CSV to OSM XML format
- `docs/import_plan.md` — full description of the import procedure
- `docs/ukrnafta_license_confirmation.pdf` — official confirmation letter (digitally signed)

## Contact

For questions or updates, please contact:

- **Email:** maps.services@ukrnafta.com
- **OSM import coordinator:** v.vlasyuk@4service-group.com

---
