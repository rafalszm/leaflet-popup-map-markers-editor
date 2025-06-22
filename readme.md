# Leaflet Popup Map Editor

**Interaktywny edytor mapowy** oparty na Leaflet z obsługą:

- dodawania i edycji markerów różnych typów (wejście, niebezpieczeństwo, obiekt),
- wyszukiwania lokalizacji po adresie,
- geolokalizacji użytkownika,
- wyboru warstwy mapy (OpenStreetMap, satelita, dark, LIDAR),
- eksportu konfiguracji (widok mapy + markery) do formatu JSON.

## ✨ Funkcje

- 🗺️ **Mapa Leaflet** z popupem modalnym i kontrolkami w stylu Google Maps.
- 📌 Dodawanie do 3 markerów danego typu z opisem i możliwością zmiany typu.
- 🧱 Przyciski w lewym górnym rogu do aktywacji trybu dodawania konkretnego typu znacznika.
- 🧹 Możliwość przesuwania i usuwania istniejących znaczników.
- 🔍 Wyszukiwarka lokalizacji (Leaflet Control Geocoder).
- 🛰 Warstwy map bazowych: standardowa mapa, satelita, ciemny motyw, LIDAR z Geoportalu.
- 📡 Przycisk lokalizacji GPS użytkownika.
- 🔐 Znacznik lokalizacji użytkownika jest nieedytowalny.
- 💾 Po zamknięciu popupu konfiguracja mapy i wszystkie znaczniki są logowane jako JSON do konsoli.

## 📦 Jak używać

1. Umieść plik `.html` na swoim serwerze lub uruchom lokalnie.
2. Kliknij „Otwórz mapę”.
3. Dodaj markery, wybierz warstwę mapy, dostosuj widok.
4. Kliknij „Zamknij” – dane zostaną zapisane w konsoli.

## 🔧 Technologie

- [Leaflet.js](https://leafletjs.com/)
- [Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder)
- Font Awesome (ikony)

## 📝 Przykład JSON (po zamknięciu)

```json
{
  "view": {
    "center": { "lat": 52.2297, "lng": 21.0122 },
    "zoom": 13,
    "baseLayer": "Mapa"
  },
  "markers": [
    {
      "lat": 52.2301,
      "lng": 21.0100,
      "type": "wejście",
      "note": "Główne wejście"
    }
  ]
}
```

---

> Projekt idealny do tworzenia szkiców map eksploracyjnych, dokumentacji terenowej lub lekkiego edytora GIS w przeglądarce.

