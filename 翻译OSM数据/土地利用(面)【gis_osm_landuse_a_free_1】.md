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
