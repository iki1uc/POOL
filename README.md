# 🧩 POOL – Globaler Datenpool

POOL ist der zentrale, globale Datenpool der gesamten AXO‑Architektur.  
Er dient als **ANKER (Stabilisierungsachse)** und als **Datenquelle**, aus der alle Module lesen können.

POOL führt **keine Berechnungen** aus.  
POOL ist **rein lesend, verwaltend, verteilend**.

---

## 🎯 Zweck

- Zentraler Speicherort für AXO‑Daten  
- Bereitstellung von Q‑Pool, Vektor‑Pool und NC‑Pool  
- Verwaltung von AXO‑IDs und AXO‑Operator‑Ergebnissen  
- Stabilisierungsachse für NC‑Hub‑All  
- Routing‑Quelle für DR  
- Datenquelle für index.html und id.html

POOL ist der **Startpunkt** der gesamten Datenarchitektur.

---

## 📦 Struktur

Das Repository enthält:

- **README.md** – Dokumentation  
- **index.html** – Frontend‑Demo, zeigt POOL‑Daten  
- **id.html** – Anzeige einzelner AXO‑IDs  
- **pool-quelle-3.csv** – Definition der drei Kernpools

---

## 📂 pool-quelle-3.csv

Pool,Quelle,Zweck
Q‑Pool,q81(v),"Qualität, Richtung, Länge"
Vektor‑Pool,"ABC_Vektor, OrbitLink, TMP81","Achse, ID, Vektor"
NC‑Pool,"NC, HDF_PATH, CACHE_UPDATE","Standort, Speicher, Routing"


Diese drei Pools bilden die **Grundlage für AXO**.

---

## 🔧 Verwendung in AXO

POOL wird von folgenden Modulen genutzt:

- **AXO_ID.js**  
- **AXO_Operator.js**  
- **AXO_LAGE_ORt.js**  
- **AXO_Final.js**  
- **NC‑Hub‑All**  
- **DR**

Beispiel:

```js
POOL.register("AXO", {
  id: axo_id,
  standort,
  vektor,
  orbit,
  qualität,
  richtung,
  länge
});
🌐 index.html
Zeigt die Inhalte des POOL‑Datenpools im Browser an.

🧩 id.html
Zeigt eine einzelne AXO‑ID als JSON‑Objekt.

🚀 Installation
bash
git clone https://github.com/iki1uc/POOL.git
cd POOL
📄 Lizenz
Dieses Projekt ist frei nutzbar.

Code

---

# ⭐ POOL ist jetzt **fertig**  
Du hast jetzt:

- **AXO fertig**  
- **POOL fertig**  
- **NC‑Hub‑All fertig**  
- **DR fertig**  
- **README.md fertig**  
- **index.html + id.html kompatibel**

