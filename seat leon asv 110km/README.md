# Seat Leon 1.9 TDI ASV 110 KM - EDC15VM+

## Identyfikacja ECU:
* **ECU:** Bosch EDC15VM+
* **Nr Bosch:** 0281011312
* **Wersja oprogramowania:** 1037367049
* **Nr VAG:** 038906012HD
* **Skrzynia:** Manualna (Codeblock 2 / Coding 00002)
* **Rozmiar pamięci:** 512 KB (524 288 bajtów)

---

## Zawartość folderu:
1. **`38906012HD-SG  4890 Seat Leon.Bin`**
   * Oryginalny fabryczny wsad (ORI).
2. **`seatnapierdalankav2.bin`**
   * Zmodyfikowana mapa (Stage 1+ Extreme Popcorn & Flames).

---

## Modyfikacje w `seatnapierdalankav2.bin`:
* **Agresywna odcinka / Popcorn limiter (ratatatata):**
  * Torque Limiter: 4450 RPM (70.0 mg) $\rightarrow$ 4500 RPM (0.0 mg) – 50 RPM skoku zoptymalizowane pod bezwładność nastawnika VP37.
  * Smoke Limiter 1 & 2: 4450 RPM (70.0 mg) $\rightarrow$ 4500 RPM (0.0 mg).
* **Płomienie z wydechu (Exhaust Flames):**
  * Kąt wtrysku (SOI): przesunięta oś obrotów na 4350 RPM.
  * Od 4350 RPM do 5355 RPM kąt wtrysku wynosi **-6.00° po GMP (ATDC)** na wszystkich mapach od 10°C do 86°C.
  * Wtrysk 70 mg w fazie wydechu prosto w rozgrzaną turbinę i kolektor.
* **Napięcia pompy VP37 (N146):**
  * Podbicie napięcia przy 3500–4500 RPM do maksymalnego bezpiecznego zakresu mechanicznego tłoczka 10mm:
    * 35 mg: **4.39 V** (3600 raw)
    * 40 mg: **4.64 V** (3800 raw)
    * 65 mg: **4.76 V** (3900 raw) – maksymalny wydatek fali przed błędem nastawnika (DTC 01268).
* **Odblokowany limiter dymu na postoju (Free Rev):**
  * Komórki niskiego przepływu powietrza (300–500 mg/stroke) odblokowane na wysokich obrotach do 70 mg (pozwala na pełne strzały bez doładowania na biegu jałowym).
* **Doładowanie Turbo (VNT):**
  * Ciśnienie zadane podniesione do 2550 mbar (1.55 bar boost).
  * Ogranicznik Single Value Boost Limit (SVBL) ustawiony na 2720 mbar.
  * Korekta N75 dla szybszego wstawania turbiny (spool boost).
* **EGR 100% OFF:**
  * Wartości 8500 wpisane w całą mapę MAF oraz dodatkowe krzywe (0x75096 – 0x7529C).
* **Poprawa odpalania (Start IQ):**
  * +12% dawki startowej na ciepłym i zimnym silniku (likwidacja problemu ciepłego rozruchu w 1.9 TDI).
* **Sumy kontrolne (Checksums):**
  * 5/5 zgodne wg algorytmu Bosch 2002 EDC15VM (przeliczone i zweryfikowane).
