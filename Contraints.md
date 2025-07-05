# 📊 SQL Constraints: Column-level vs Table-level

| Constraint       | Column Level ✅ | Table Level ✅ | Description                                                     |
| ---------------- | -------------- | ------------- | --------------------------------------------------------------- |
| `NOT NULL`       | ✅ Yes          | ❌ No          | Ensures the column cannot have `NULL` values                    |
| `DEFAULT`        | ✅ Yes          | ❌ No          | Sets a default value for the column                             |
| `UNIQUE`         | ✅ Yes          | ✅ Yes         | Ensures all values in the column or group of columns are unique |
| `PRIMARY KEY`    | ✅ Yes (1 col)  | ✅ Yes         | Uniquely identifies each row — must be NOT NULL & UNIQUE        |
| `FOREIGN KEY`    | ❌ No           | ✅ Yes         | Links column(s) to primary key in another table                 |
| `CHECK`          | ✅ Yes          | ✅ Yes         | Ensures a condition is true for values                          |
| `AUTO_INCREMENT` | ✅ Yes (MySQL)  | ❌ No          | Auto-generates increasing numeric values (MySQL only)           |
