### 调优技巧

1. 执行顺序：on > where > having
2. 执行顺序：在group by中，where > having
3. 用exists替换in，但not exists与no in不相等
4. 关联时小表在前，小表会放入到内存中。
5. where后的条件执行顺序为逆序，故将可以过滤掉大部分数据的条件写在后边。
6. 避免使用耗资源的操作，如distinct、union、minus、order by，这几个都需要进行排序操作，占资源较大。
7. 索引列不作计算操作。