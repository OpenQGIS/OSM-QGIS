**gis_osm_roads_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'bridleway' THEN '骑行道（马）'
    WHEN "fclass" = 'cycleway' THEN '自行车道'
    WHEN "fclass" = 'footway' THEN '步行道'
    WHEN "fclass" = 'living_street' THEN '生活性街道'
    WHEN "fclass" = 'motorway' THEN '高速路'
    WHEN "fclass" = 'motorway_link' THEN '高速匝道'
    WHEN "fclass" = 'path' THEN '小道'
    WHEN "fclass" = 'pedestrian' THEN '步行街'
    WHEN "fclass" = 'primary' THEN '主要道;省道'
    WHEN "fclass" = 'primary_link' THEN '主要道连接线;省道连接线'
    WHEN "fclass" = 'residential' THEN '住宅道路'
    WHEN "fclass" = 'secondary' THEN '次要道'
    WHEN "fclass" = 'secondary_link' THEN '次要道连接线'
    WHEN "fclass" = 'service' THEN '服务道路'
    WHEN "fclass" = 'steps' THEN '台阶'
    WHEN "fclass" = 'tertiary' THEN '三级道路'
    WHEN "fclass" = 'tertiary_link' THEN '三级道路连接线'
    WHEN "fclass" like 'track%' THEN '土路'
    WHEN "fclass" = 'trunk' THEN '国道;快速路'
    WHEN "fclass" = 'trunk_link' THEN '国道连接线;快速路连接线'
    WHEN "fclass" = 'unclassified' THEN '等级外道路'
    WHEN "fclass" = 'unknown' THEN '不知名道路'
    ELSE '其他'
/* Copyright by OpenQGIS */
END
~~~

