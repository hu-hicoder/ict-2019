# SQL
- note https://www.w3schools.com/sql/exercise.asp w3schoolをやりました。学んだことをメモしています。
- **DISTINCT**
- different value
```
SELECT DISTINCT column1, column2,... FROM table_name;
```
- **NOT**
- 否定
```
SELECT * FROM Customers WHERE NOT City = 'Berlin';
```
- **WHERE**
```
... WHERE City = 'Berlin' OR City = 'London';
```
- **ORDER BY**
- sortする
```
SELECT ... table ORDER BY column; 
```
- reverse sort
```
ORDER BY column DESC
```
- multi
```
ORDER BY column1, column2, ...
```
- **INSERT**
```
INSERT INTO table (
    column1,
    column2
)
VALUES (
    value1,
    value2
);
```
- **NULL**
```
WHERE column IS NULL;
```
- **UPDATE**
```
UPDATE table SET column1 = 'String', column2 = 'String' WHERE column = 'String';
```
- **DELETE**
```
DELETE FROM table WHERE column = 'String';
```
- **MIN, MAX, COUNT**
```
SELECT MIN(column) FROM table;
SELECT MAX(column) FROM table;
SELECT COUNT(*) FROM table WHERE column = 'Value';
SELECT AVG(column) FROM table;
SELECT SUM(column) FROM table;
```
- **LIKE**
```
SELECT * FROM table WHERE column LIKE 'a%';　# aからはじまるもの
NOT LIKE 'a%' # aから始まらないもの
LIKE '_a%' # 2nd letter a
LIKE '[acs]%'; # starts 'a or c or s'
LIKE '[a-f]%'; # starts a-f
LIKE '[^acf]%' # not start acf
```
- **IN, BETWEEN**
- between alphabetical order is OK
```
SELECT * FROM table WHERE column IN ('String1', 'String2'); # column==String1 or String2
NOT IN # NOT
WHERE column BETWEEN value1 AND value2; # between 10-20
NOT BETWEEN; NOT
```
- **ALIAS**
```
SELECT column1, column2 AS AAA, column3 FROM table; # ASでALIASできる
# tableもALIASできる
```
- **JOIN**
- INNER JOIN, LEFT JOIN, RIGHT JOIN,
- **GROUP BY**
```
SELECT COUNT(column), column FROM table GROUP BY column;
```
- **DATABASE**
```
CREATE DATABASE name;
DROP DATABASE name;
TRUNCATE TABLE name; # テーブル内データ消去
ALTER TABLE name ADD a b; #  add a column type b, called a
ALTER TABLE a DROP COLUMN b # aからbというcolumnを消す
```
# plus
- Stringは`''`でくくる

# 参考
- https://www.w3schools.com/sql/exercise.asp ここをやりました。