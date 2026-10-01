# Mapsforge POI Multi-language Mapping

Resources and optimized data for the internationalization  of Points of Interest (POI) in **Mapsforge** vector maps and compatible apps (**OruxMaps**, **Cruiser**).

## 📌 What is this about?
Transforms and structures the original configuration file from [mapsforge-poi-writer poi-mapping.xml](https://github.com/mapsforge/mapsforge/blob/master/mapsforge-poi-writer/src/main/config/poi-mapping.xml) into accessible, multi-language formats for developers.

## 📂 Main Files

  ### `poi-mapping.xml`
An adapted version of the original `poi-mapping.xml` where multilingual support has been integrated directly into the categories using child `<translation lang="...">` elements for German (`de`), Spanish (`es`), French (`fr`), Italian (`it`), and Dutch (`nl`), serving as a solid foundation for future automation via scripts or other tools.

* **Structure:** Keeps the English name in the `title` attribute and nests the localized translations using individual `<translation>` tags for each language.
* **Preservation:** Keeps all original comments (`<!--`) and the original file structure completely intact .

