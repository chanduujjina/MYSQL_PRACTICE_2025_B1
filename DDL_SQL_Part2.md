# Create table

## ✅ Sample Syntax (Without Constraints)
```sql
CREATE TABLE table_name (
    column1 data_type,
    column2 data_type,
    column3 data_type,
    ...
);
```
## 🔁 2. Rename Table
```sql
RENAME TABLE old_table_name TO new_table_name;
```

## ❌ 3. Delete All Rows from Table (But Keep Structure)
```sql
DELETE FROM table_name;
```

## 🧨 4. Drop Table (Delete Table Completely)
```sql
DROP TABLE table_name;
```
## 🧠 Summary Table
| Task         | Generic SQL Command                        |
| ------------ | ------------------------------------------ |
| Create Table | `CREATE TABLE table_name (...)`            |
| Rename Table | `RENAME TABLE old TO new` or `ALTER TABLE` |
| Delete Data  | `DELETE FROM table_name`                   |
| Drop Table   | `DROP TABLE table_name`                    |

