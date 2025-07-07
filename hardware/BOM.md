# 3DBuddy – Bill of Materials (BOM)

All prices are July 2025 retail / 1-off **incl. Danish VAT** (shipping excluded).

## 1. Tavlekomponenter (WATTO.dk)

| Qty | Item | Unit price | Sub-total |
|----:|------|-----------:|----------:|
| 3 | [Schneider Resi9 MCB 1P+N C10 A 6 kA 18 mm R9P19610](https://watto.dk) | 34 kr | 102 kr |
| 1 | [Schneider Resi9 RCBO 1P+N C13 A 6 kA 30 mA R9D55613](https://watto.dk) | 297 kr | 297 kr |
| 2 | [Eastron SDM120D MID kWh-måler 45 A 1-modul](https://watto.dk) | 200 kr | 400 kr |
| 1 | [Kontaktor 25 A 4 NO 24 VAC coil](https://watto.dk) | 270 kr | 270 kr |
| 1 | [Mean Well HDR-30-24 DIN-PSU 24 V 1 - 1.25 A SELV](https://watto.dk) | 255 kr | 255 kr |
| 1 | DIN-skinne 35 mm 260 mm | 30,5 kr | 30,5 kr |
| 44 | WAGO / Weidmüller WDU 2,5 mm² gennemgangsklemmer | 5,8 kr | 255,2 kr |

**Del­sum tavle:** **1 609,7 kr**

---

## 2. Fælleskomponenter for begge kabinetter (WATTO.dk)

| Qty | Item | Unit price | Sub-total |
|----:|------|-----------:|----------:|
| 2 | [Phoenix Contact EO-CF/PT servicestik (Push-in)](https://watto.dk) | 51,5 kr | 103 kr |
| 1 | Schuko stikdåse 8 udtag med jord | 93 kr | 93 kr |
| 1 | [Schneider nødstop Ø40 mm XB5AS8445](https://watto.dk) | 289 kr | 289 kr |

**Del­sum fælles:** **485 kr**

---

## 3. PLC (Controllino.com)

| Qty | Item | Unit price | Sub-total |
|----:|------|-----------:|----------:|
| 1 | [CONTROLLINO MINI 24 V PLC](https://controllino.com/product/controllino-mini) | 139 EUR (~1 100 kr) | ~1 100 kr |

---

## 4. Elektronik til kabinet A + B (2 kamre)

| Qty | Item | Unit price | Sub-total |
|----:|------|-----------:|----------:|
| 4 | [Sunon MEC0382V3-000U-A99 120 mm 24 V blæser (93 CFM)](https://www.tme.eu/en/details/mec0382v3-000u-a99/dc-fans/sunon/) | 120 kr | 480 kr |
| 2 | [SHT31-D STEMMA QT Temp/RH-sensor](https://www.adafruit.com/product/4022) | 95 kr | 190 kr |
| 2 | [SGP40 STEMMA QT VOC-sensor](https://www.adafruit.com/product/4829) | 105 kr | 210 kr |
| 2 | [Fermion MEMS Smoke-sensor SEN0570](https://www.dfrobot.com/product-2246.html) | 35 kr | 70 kr |
| 2 | [Grove magnet-reed-switch](https://www.seeedstudio.com/Grove-Magnetic-Switch-p-426.html) | 23 kr | 46 kr |
| 2 | [Grove RGB-LED Stick (15 × WS2813)](https://www.seeedstudio.com/Grove-RGB-LED-Stick-WS2813-15-LEDs-p-3122.html) | 45 kr | 90 kr |

**Del­sum kabinetter:** **1 086 kr**

---

## 5. Kabler & ledninger (meterpriser)

| Behov | Kabeltype | Pris pr. meter/pack | Leverandør |
|-------|-----------|--------------------|------------|
| 70 m | [H07V-K 1,5 mm² (5 farver)](https://uk.rs-online.com/web/p/hook-up-wire/0361822) | 6 kr/m | RS Components |
| 50 m | [LiYY 4 × 0,34 mm² multicore](https://dk.farnell.com/lapp-kabel/0028404) | 7,5 kr/m | Farnell |
| 2 × 5 stk | [Grove/JST-QT 4-pin patch 0,5 m](https://store-usa.arduino.cc/products/grove-universal-4-pin-buckled-50cm-cable-5-pcs) | 24 kr/pk | Arduino Store |

---

### **Samlet hardware-overslag:** ~**5 100 kr** (ekskl. fragt)

---

## CE- & lovgivnings­overblik

| Omfang | Primære EU-direktiver | Centrale EN-standarder | Praktisk to-do |
|--------|----------------------|------------------------|----------------|
| **Tavle (230 V DIN-skab)** | • Lavspænding (2014/35/EU)<br>• EMC (2014/30/EU)<br>• RoHS (2011/65/EU) | EN 61439-1/-2 (lavspændingstavler) | • Mærkeskilt med U_n, I_n, IP20 + CE<br>• PE- & isolationstest (EN 60204-1 §18) |
| **Lavspændings-ø (< 60 V DC)** | • EMC<br>• RoHS | EN 61000-6-2/-4 (industri EMC) | • SELV-adskillelse fra 230 V<br>• Kabelføring: adskil I²C fra netledninger |
| **Maskine (2 kamre + tavle)** | • EMC<br>• *Evt.* Maskindirektivet 2006/42/EF (eller 2023/1230) ved kommercielt salg | EN 60204-1 (el-udstyr), EN ISO 12100 (risikoanalyse), EN 13849-1 (nødstop) | • Udarbejd risikoanalyse & DoC<br>• Dokumentér at RCBO + nødstop afbryder på < 0,5 s |
| **MID** | – (kWh-måler er allerede MID-certificeret) | – | Behold fabrikantens DoC i teknisk dossier |
| **RF / RED** | – (ingen trådløs modul i den valgte konfiguration) | – | – |

> **Kort sagt:**  
> * Saml alle fabrikants-DoC’er som bilag.  
> * Byg tavlen efter EN 61439-1/-2, udfør el-test og fastgør CE-mærkeplade.  
> * Lav en kort manual + samlet EU-overensstemmelses­erklæring for hele systemet.  
> * EMC-risiko minimeres ved god kabelføring og skærmet LiYY til I²C-bus.

---

*Sidst opdateret: **07-07-2025** – tilpas priser og links efter behov.*
