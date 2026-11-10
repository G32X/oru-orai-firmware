# Orų Orai – programinės įrangos atnaujinimai ir atviri duomenys

Šiame repo yra sukompiliuota „Orų Orai“ programa Waveshare ESP32-S3-Touch-LCD-7B ekraniukui (`firmware.bin`, `version.json`).
Ekraniukai ją atsisiunčia per Wi-Fi: **Nustatymai → Programinė įranga**.

## Ekrano kopijos

| | |
|---|---|
| ![Orai](screenshots/01-orai.png) | ![Vėjas ir valandinė prognozė](screenshots/02-vejas-valandos.png) |
| Orų žemėlapis ir dabartiniai orai | Vėjo žemėlapis ir valandinė prognozė |
| ![Krituliai ir savaitė](screenshots/03-krituliai-savaite.png) | ![Radaras](screenshots/04-radaras.png) |
| Kritulių žemėlapis ir savaitės prognozė | Kritulių radaras (tiesiogiai ir 2 val. istorija) |
| ![Paieška](screenshots/05-paieska.png) | ![Užsklanda](screenshots/06-uzsklanda.png) |
| Vietovės paieška (2324 LHMT vietovės) | Užsklanda |

## Orų duomenys (LHMT, CC BY-SA 4.0)

Prognozės, faktiniai stebėjimai ir vietovių bei stočių sąrašas gaunami iš
**Lietuvos hidrometeorologijos tarnybos prie Aplinkos ministerijos (LHMT)**: <https://api.meteo.lt>.

Duomenys naudojami pagal licenciją **Creative Commons Priskyrimas–Analogiškas platinimas 4.0 tarptautinė (CC BY-SA 4.0)**:
<https://creativecommons.org/licenses/by-sa/4.0/legalcode.lt>.

Duomenys yra pakeisti:
- reikšmės suapvalintos;
- parenkama artimiausia prognozės valanda;
- duomenys sugrupuoti pagal dienas;
- duomenys pavaizduoti ikonomis, grafiku ir žemėlapyje.

Ekraniuke rodomi išvestiniai orų duomenys taip pat platinami pagal CC BY-SA 4.0.

Duomenys teikiami „tokie, kokie yra“, be jokių garantijų. LHMT neatsako už duomenų tikslumą ir jų naudojimo pasekmes.
LHMT šio produkto neremia ir su juo nesusijusi.

### Programinėje įrangoje įdiegti LHMT duomenys

Programinėje įrangoje įdiegti du LHMT sąrašai, jie čia pateikti atvirai pagal **CC BY-SA 4.0**:

| Failas | Turinys | Šaltinis | Pakeitimai |
|---|---|---|---|
| [`places.csv`](places.csv) | 2324 Lietuvos vietovės: kodas, pavadinimas, savivaldybė, koordinatės | <https://api.meteo.lt/v1/places> | atrinktos Lietuvos vietovės, surikiuotos pagal pavadinimą, pridėtas paieškos raktas `search_key` (be diakritikų) |
| [`stations.csv`](stations.csv) | 52 LHMT meteorologijos stotys: kodas, pavadinimas, koordinatės | <https://api.meteo.lt/v1/stations> | konvertuota į CSV |

## Kiti duomenys

- **Kritulių radaras:** Weather data by RainViewer, <https://www.rainviewer.com>. Radaro duomenis teikia nacionalinės meteorologijos tarnybos, žr. <https://www.rainviewer.com/sources.html>.
- **Žemėlapis:** Made with Natural Earth (viešasis domenas), <https://www.naturalearthdata.com>.

## Atviro kodo komponentai

Pranešimai ir licencijos aprašyti [`NOTICE.md`](NOTICE.md). Pilni licencijų tekstai yra kataloge [`licenses/`](licenses/).
