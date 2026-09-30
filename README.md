# Mapsforge POI Multi-language Mapping

Resources and optimized data for the internationalization  of Points of Interest (POI) in **Mapsforge** vector maps and compatible apps (**OruxMaps**, **Cruiser**).

## 📌 What is this about?
Transforms and structures the original configuration file from [mapsforge-poi-writer poi-mapping.xml](https://github.com/mapsforge/mapsforge/blob/master/mapsforge-poi-writer/src/main/config/poi-mapping.xml) into accessible, multi-language formats for developers.

## 📂 Main Files
* `poi-mapping-translations-v1.json`: JSON structure containing categories, OpenStreetMap tags, and translations (v1).

## 🌍 Languages (v1)
* 🇬🇧 **English** (Base)
* 🇪🇸 **Spanish** (`es`)
* 🇩🇪 **German** (`de`)
* 🇫🇷 **French** (`fr`)
* 🇮🇹 **Italian** (`it`)
* 🇳🇱 **Dutch** (`nl`)

* `poi-mapping-translations-v2.json`: JSON structure containing categories, OpenStreetMap tags, and translations (v2).

## 🌍 Languages (v2)
* 🇬🇧 **English** (Base)
* 🇷🇺 **Russian** (`ru`)
* 🇨🇿 **Czech** (`cs`)
* 🇵🇹 **Portuguese** (`pt`)
* 🇸🇻 **Swedish** (`sv`)

### `Poi-mapping-multilanguage.xml`
An adapted version of the original `poi-mapping.xml` that incorporates multilingual support into POI categories as a foundation for the future, easily modifiable via scripts or other tools.

* **Attribute Order:** `title` (English), `title_de`, `title_es`, `title_fr`, `title_it`, and `title_nl`.
* **Preservation:** Keeps (or so I aim :) all original comments (`<!--`) and the original file structure completely intact.

  ### `poi-mapping-translation.xml`
An adapted version of the original `poi-mapping.xml` where multilingual support has been integrated directly into the categories using child `<translation lang="...">` elements for German (`de`), Spanish (`es`), French (`fr`), Italian (`it`), and Dutch (`nl`), serving as a solid foundation for future automation via scripts or other tools.

* **Structure:** Keeps the English name in the `title` attribute and nests the localized translations using individual `<translation>` tags for each language.
* **Preservation:** Keeps all original comments (`<!--`) and the original file structure completely intact while expanding specialized outdoor and OAM categories (Tourism, Waterways, and Bicycle-related infrastructure).

