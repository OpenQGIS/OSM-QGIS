**gis_osm_waterways_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'river' THEN '河流'
    WHEN "fclass" = 'stream' THEN '溪流'
    WHEN "fclass" = 'canal' THEN '运河'
    WHEN "fclass" = 'drain' THEN '排水沟'
    ELSE '其他'
    /* Copyright by OpenQGIS */
END
~~~
