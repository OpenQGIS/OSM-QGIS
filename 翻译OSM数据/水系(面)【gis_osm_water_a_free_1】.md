**gis_osm_water_a_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'water' THEN '水体'
    WHEN "fclass" = 'reservoir' THEN '水库'
    WHEN "fclass" = 'river' THEN '河流'
    WHEN "fclass" = 'dock' THEN '码头'
    WHEN "fclass" = 'glacier' THEN '冰川'
    WHEN "fclass" = 'wetland' THEN '湿地'
    ELSE '其他'
END
/* Copyright by OpenQGIS */
~~~
