# kokain_EU

## TXT file

```bash

Ausztria;1995.01.01
Belgium;1958.01.01
Bulg�ria;2007.01.01
Ciprus;2004.05.01
Csehorsz�g;2004.05.01
D�nia;1973.01.01
Egyes�lt Kir�lys�g;1973.01.01
�sztorsz�g;2004.05.01
Finnorsz�g;1995.01.01
Franciaorsz�g;1958.01.01
G�r�gorsz�g;1981.01.01
Hollandia;1958.01.01
Horv�torsz�g;2013.07.01
�rorsz�g;1973.01.01
Lengyelorsz�g;2004.05.01
Lettorsz�g;2004.05.01
Litv�nia;2004.05.01
Luxemburg;1958.01.01
Magyarorsz�g;2004.05.01
M�lta;2004.05.01
N�metorsz�g;1958.01.01
Olaszorsz�g;1958.01.01
Portug�lia;1986.01.01
Rom�nia;2007.01.01
Spanyolorsz�g;1986.01.01
Sv�dorsz�g;1995.01.01
Szlov�kia;2004.05.01
Szlov�nia;2004.05.01
```

```python
exec('from collections import Counter\nwith open("EUcsatlakozas.txt","r", encoding="latin2") as f: lista = [sor.strip().split(";") for sor in f]; print(f"""3.feladat: EU tagállamainak száma: {len(lista)} db.\n4.feladat: 2007-ben {len([sor for sor in lista if sor[1][:4]=="2007"])} ország csatlakozott\n5.feladat: Magyarország csatlakozási dátuma: {[sor[1] for sor in lista if sor[0]=="Magyarország"][0]}\n6.feladat: Májusban {"van" if [sor for sor in lista if sor[1][5:7] == "05"] else "nincs"} csatlakozás\n7.feladat: Legutoljára csatlakozott ország: {max(lista, key=lambda adat : adat[1])[0]}!\n8.feladat: statisztika""")\n[print(f"{ev} - {db} ország") for ev, db in [Counter(sor[1][0:4] for sor in lista)][0].items()]') #egy sor XDDDD
```
## *'egy sor'* XDD
