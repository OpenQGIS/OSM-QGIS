**gis_osm_railways_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'rail' THEN '铁路'
    WHEN "fclass" = 'light_rail' THEN '轻轨'
    WHEN "fclass" = 'subway' THEN '地铁'
    WHEN "fclass" = 'tram' THEN '电车'
    WHEN "fclass" = 'monorail' THEN '单轨'
    WHEN "fclass" = 'narrow_gauge' THEN '窄轨'
    WHEN "fclass" = 'miniature' THEN '微型铁路'
    WHEN "fclass" = 'funicular' THEN '缆索铁路'
    WHEN "fclass" = 'rack' THEN '齿轨铁路'
    WHEN "fclass" = 'drag_lift' THEN '拖牵'
    WHEN "fclass" = 'chair_lift' THEN '座椅缆车'
    WHEN "fclass" = 'cable_car' THEN '缆车'
    WHEN "fclass" = 'gondola' THEN '缆车吊舱'
    WHEN "fclass" = 'goods' THEN '货运缆车'
    WHEN "fclass" = 'other_lift' THEN '其他缆车'
    ELSE '其他'
    /* Copyright by OpenQGIS */
END
~~~
