# kokain_EU

```python
exec('from collections import Counter\nwith open("EUcsatlakozas.txt","r", encoding="latin2") as f: lista = [sor.strip().split(";") for sor in f]; print(f"""3.feladat: EU tagállamainak száma: {len(lista)} db.\n4.feladat: 2007-ben {len([sor for sor in lista if sor[1][:4]=="2007"])} ország csatlakozott\n5.feladat: Magyarország csatlakozási dátuma: {[sor[1] for sor in lista if sor[0]=="Magyarország"][0]}\n6.feladat: Májusban {"van" if [sor for sor in lista if sor[1][5:7] == "05"] else "nincs"} csatlakozás\n7.feladat: Legutoljára csatlakozott ország: {max(lista, key=lambda adat : adat[1])[0]}!\n8.feladat: statisztika""")\n[print(f"{ev} - {db} ország") for ev, db in [Counter(sor[1][0:4] for sor in lista)][0].items()]') #egy sor XDDDD
```
## egy sor XDD
