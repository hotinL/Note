# 批量更新

```mysql
EXPLAIN UPDATE t_shop 
SET shop_view = CASE 
WHEN shop_id = 2 THEN 2 
WHEN shop_id = 3 THEN 1
END 
WHERE shop_id IN ( 2 , 3 ) 
```

