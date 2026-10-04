# Audi A4 B6 1.8T BFB 163 KM - Wsady Sterownika ME7.5

Folder zawiera wsady do sterownika Bosch ME7.5 z silnika Audi A4 B6 1.8 Turbo 20V (kod silnika BFB, 163 KM / 120 kW).

---

## 📁 Zawartość folderu:

1. **`1.8T BFB ORI` / `1.8T BFB ORI.bin`** (Plik z Pulpitu):
   - **Modyfikacja**: **2 SONDA LAMBDA OFF (Post-cat Lambda / Decat OFF)**.
   - Posiada wyłączoną diagnostykę oraz wyłączoną grzałkę drugiej sondy lambda za katalizatorem w konfiguracji końcówek mocy (**ESKONF** pod adresami `0x10D9E`, `0x10DA2`, `0x10DAF` zmienione na `0x00`).
   - Pozwala na jazdę bez katalizatora (downpipe / decat) bez wywalania Check Engine i błędów P0420, P0140, P0141.
   - Sumy kontrolne (ME7Sum / ME7Check) są w 100% przeliczone i poprawne.

2. **`1.8T BFB FABRYCZNY 100% SERIA.bin`**:
   - Fabryczny, w 100% oryginalny wsad z fabryczną aktywną 2 sondą i seryjnymi sumami producenta.

---

## 🔍 Identyfikacja sterownika (ECUID):
- **Silnik**: 1.8T 20V (1.8L R4/5VT) - BFB 163 KM (120 kW)
- **Sterownik**: Bosch ME7.5
- **Numer Bosch HW (SSECUHN)**: `0261207934`
- **Numer Bosch SW (SSECUSN)**: `1037366494`
- **Numer części VAG**: `8E0909518AA`
- **Wersja oprogramowania VAG**: `0004`
- **Wersja Bootrom**: `06.02`
- **Sygnatura EPK**: `40/1/ME7.5/5/4016.32//24G/Dst04o/080802//`
- **Rozmiar pamięci**: 1 048 576 bajtów (1024 KB Flash 29F800BT)
- **Status Checksum**: Zweryfikowane, pliki w 100% sprawne i bezpieczne.
