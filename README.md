# grassleanings

Mike's grass lessons

https://twitter.com/pierreroudier/status/1420898335343333380?s=20

etc. 


```
grass  -c EPSG:7844 ~/grassdata/abs
v.import abs/ASGS_2021_Main_Structure_GDA2020.gpkg   output=ASGS_2021_Main_Structure_GDA2020 --o


grass -c EPSG:7844 ~grassdata/test
v.import input=abs/ASGS_2021_Main_Structure_GDA2020.gpkg layer=AUS_2021_AUST_GDA2020 output=AUS_2021_AUST_GDA2020 

v.generalize input=AUS_2021_AUST_GDA2020 output=simple method=douglas threshold=2000
v.out.ogr input=simple type=area output=simple.gpkg

```
