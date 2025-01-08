# OSM-QGIS
使用QGIS解读OSM原始数据，主要包括*.pbf和*.osm数据读取；将osm各项数据做中文属性翻译

## OSM部分属性翻译
### 翻译OSM道路数据
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

### 翻译OSM土地利用
**gis_osm_landuse_a_free_1**<br>
注：属性表表头为fclass

~~~
CASE 
    WHEN "fclass" = 'forest' THEN '森林'
    WHEN "fclass" = 'park' THEN '公园'
    WHEN "fclass" = 'residential' THEN '住宅区'
    WHEN "fclass" = 'industrial' THEN '工业区'
    WHEN "fclass" = 'cemetery' THEN '墓地'
    WHEN "fclass" = 'allotments' THEN '配给地'
    WHEN "fclass" = 'meadow' THEN '草地'
    WHEN "fclass" = 'commercial' THEN '商业区'
    WHEN "fclass" = 'nature_reserve' THEN '自然保护区'
    WHEN "fclass" = 'recreation_ground' THEN '游乐场'
    WHEN "fclass" = 'retail' THEN '零售区'
    WHEN "fclass" = 'military' THEN '军事区'
    WHEN "fclass" = 'quarry' THEN '采石场'
    WHEN "fclass" = 'orchard' THEN '果园'
    WHEN "fclass" = 'vineyard' THEN '葡萄园'
    WHEN "fclass" = 'scrub' THEN '灌木丛'
    WHEN "fclass" = 'grass' THEN '草地'
    WHEN "fclass" = 'heath' THEN '荒地'
    WHEN "fclass" = 'national_park' THEN '国家公园'
    WHEN "fclass" = 'farmland' THEN '农田'
    WHEN "fclass" = 'farmyard' THEN '农场'
    ELSE '其他'
END
~~~

