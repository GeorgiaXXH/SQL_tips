# 1. multi_column subquery
    where (col_a, col_b) IN (select max(col_a),min(col_b) from table_a)
