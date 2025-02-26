### 🏠 **Analýza pronájmů bytů v Ostravě**  

Tento projekt se zaměřuje na **web scraping a analýzu dat o pronájmech bytů v Ostravě**.  
Cílem bylo získat informace o nabídkách bytů, zpracovat je a provést **analýzu průměrných cen a velikostí**.  
Součástí bylo také **identifikovat nejdražší lokality** a vizualizovat výsledky pomocí grafů.  

---

## 📌 **Popis problému a jeho řešení**  

Při extrakci dat jsem narazila na **problém s textovým formátem velikostí bytů** v m².  
Například: *„Pronájem bytu 2+kk 49 m²“*  
Data obsahovala **speciální znaky** (`\xa0` – pevnou mezeru), což komplikovalo zpracování.  

### 🔍 **Jak jsem problém vyřešila:**  
1. **Odstranění speciálních znaků** (`\xa0`) a jejich náhrada standardními mezerami.  
2. **Extrahování číselných hodnot** z textových řetězců pomocí regulárních výrazů.  
3. **Přidání jednotek zpět** (`m²`) pro lepší čitelnost v analýze.  

Díky těmto úvodním úpravam byla data správně připravena k analýze.  

---

## 📊 **Analýza dat**  

### 🔢 **Průměrná cena pronájmu bytu v Ostravě**  
Byla vypočtena na **13 100,12 Kč**.  

### 📅 **Průměrná cena a velikost bytů podle dispozic:**  

| Dispozice | Průměrná cena (Kč) | Průměrná velikost (m²) |
|-----------|------------------|------------------|
| **1+1** | 9 200,41 | 37,40 |
| **1+kk** | 8 724,95 | 27,77 |
| **2+1** | 11 616,59 | 56,18 |
| **2+kk** | 13 585,00 | 50,79 |
| **3+1** | 14 058,67 | 76,75 |
| **3+kk** | 20 895,09 | 80,35 |
| **4+1** | 15 580,77 | 105,31 |
| **4+kk** | 31 169,23 | 101,58 |
| **5+1** | 23 495,00 | 120,5 |
| **5+kk** | 33 050,00 | 147,00 |

**Pozorování:** Cena pronájmu **roste** s velikostí a počtem pokojů.  

### 📊 **Nejdražší lokality podle průměrného nájmu:**  

| Lokalita | Průměrná cena (Kč) |
|----------|------------------|
| **Křížkova, Ostrava - Moravská Ostrava** | 49 000,00 |
| **Šalomounova, Ostrava - Moravská Ostrava** | 46 000,00 |
| **Blahoslavova, Ostrava - Moravská Ostrava** | 39 000,00 |
| **Důlní, Ostrava - Moravská Ostrava** | 33 633,33 |
| **Keltičkova, Ostrava - Slezská Ostrava** | 33 133,33 |

**Pozorování:** Nejvyšší ceny pronájmů jsou v **Moravské Ostravě**.

---

## Vizualizace
Graf níže ukazuje průměrnou cenu pronájmu bytů v Ostravě podle dispozic.

![Průměrná cena bytu podle kompozice](https://github.com/Katy-Coder-Kat/Projekt_Python/blob/main/Graf%20byty.png?raw=true)


---

## ⚙️ **Technologie a nástroje**  

- **Python** – pandas, BeautifulSoup, re (regulární výrazy), matplotlib  
- **Web scraping** – získání dat z realitních webů  
- **Datová analýza** – čištění, zpracování a vizualizace  

---

## 💡 **Závěr**  

Data ukázala, že **ceny pronájmů se liší podle dispozic i lokalit**.  
Nejvyšší nájmy jsou v **Moravské Ostravě**, nejlevnější byty mají dispozici **1+kk a 1+1**.  

**Možné vylepšení:**  
- **Časová analýza** pro sledování změn cen v čase  
- **Získání většího vzorku dat** z více realitních webů  
