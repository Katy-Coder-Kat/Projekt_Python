# Projekt_Python
Závěrečný projekt: Analýza pronájmů bytů v Ostravě
Tento projekt se zaměřuje na web scraping a analýzu dat o pronájmech bytů v Ostravě. Cílem bylo získat informace o nabídce bytů, zpracovat je a provést analýzu průměrných cen a velikostí. Součástí bylo také identifikovat nejdražší lokality a zobrazit data v přehledných grafech.
________________________________________
Popis problému a jeho řešení
Narazila jsem na problém s extrakcí hodnot velikosti bytů v m² z textových řetězců (např. "Pronájem bytu 2+kk 49 m²"). Hodnoty obsahovaly speciální znak \xa0 (pevnou mezeru), který způsoboval problémy při zpracování dat.
Jak jsem problém vyřešila:
1.	Nejprve jsem odstranila všechny speciální znaky, jako je \xa0, a nahradila je standardními mezerami.
2.	Pomocí regulárních výrazů jsem extrahovala číselné hodnoty velikostí bytů.
3.	Pro lepší čitelnost jsem přidala zpět jednotku "m²".
Díky těmto krokům jsem zajistila správné zpracování dat a mohla pokračovat v analýze.
________________________________________
Analýza dat
1. Průměrná cena bytů
Průměrná cena pronájmů bytů v Ostravě byla vypočtena na 13 100,12 Kč.
2. Průměrná cena a velikost podle kompozice
Následující tabulka ukazuje průměrnou cenu a velikost bytů podle jejich dispozice:
Kompozice	Průměrná cena (Kč)	Průměrná velikost (m²)
1+1	9 200,41	37,40
1+kk	8 724,95	27,77
2+1	11 616,59	56,18
2+kk	13 585,00	50,79
3+1	14 058,67	76,75
3+kk	20 895,09	80,35
4+1	15 580,77	105,31
4+kk	31 169,23	101,36
5+1	23 495,00	121,00
5+kk	33 050,00	147,00
3. Nejdražší lokality
Tabulka ukazuje 5 lokalit s nejvyšší průměrnou cenou pronájmu:
Lokalita	Průměrná cena (Kč)
Křižíkova, Ostrava - Moravská Ostrava	49 000,00
K Šalomounu, Ostrava - Moravská Ostrava	46 000,00
Blahoslavova, Ostrava - Moravská Ostrava	39 000,00
Důlní, Ostrava - Moravská Ostrava	33 633,33
Keltičkova, Ostrava - Slezská Ostrava	33 133,33
________________________________________
Vizualizace
Graf: Průměrná cena a velikost bytů podle kompozice 
Tento graf ukazuje, že cena pronájmů roste s velikostí a počtem pokojů
