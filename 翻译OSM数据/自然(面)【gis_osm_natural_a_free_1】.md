**gis_osm_natural_a_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'glacier' THEN '冰川'
    WHEN "fclass" = 'peak' THEN '山峰'
    WHEN "fclass" = 'clif' THEN '悬崖'
    WHEN "fclass" = 'volcano' THEN '火山'
    WHEN "fclass" = 'tree' THEN '树'
    WHEN "fclass" = 'mine' THEN '矿井'
    WHEN "fclass" = 'cave_entrance' THEN '洞穴入口'
    WHEN "fclass" = 'beach' THEN '海滩'
    ELSE '其他'
    /* Copyright by OpenQGIS */
END
~~~

