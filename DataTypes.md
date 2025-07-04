
# Data types in SQL
## 📦 1. Numeric Data Types

| Data Type                     | Description                          | Example             |
| ----------------------------- | ------------------------------------ | ------------------- |
| `INT` / `INTEGER`             | Whole numbers (positive/negative)    | `-10`, `100`        |
| `SMALLINT`                    | Smaller range of whole numbers       | `-32,768 to 32,767` |
| `BIGINT`                      | Very large integers                  | `> 2 billion`       |
| `DECIMAL(p, s)`               | Fixed-point number                   | `123.45`            |
| `NUMERIC(p, s)`               | Same as `DECIMAL`, high precision    | `1000.01`           |
| `FLOAT`                       | Approximate decimal (floating point) | `3.14159`           |
| `REAL`                        | Less precise float                   | `3.14`              |
| `DOUBLE` / `DOUBLE PRECISION` | Higher precision float               | `3.14159265`        |
| `TINYINT`                     | Very small integer                   | `0–255`             |

## 🅰️ 2. Character/String Data Types
| Data Type            | Description                            | Example          |
| -------------------- | -------------------------------------- | ---------------- |
| `CHAR(n)`            | Fixed-length string                    | `'A'`, `'AB   '` |
| `VARCHAR(n)`         | Variable-length string (max `n` chars) | `'Hello'`        |
| `TEXT`               | Long text data                         | Articles, Notes  |
| `NCHAR` / `NVARCHAR` | Unicode characters (multilingual)      | `हिन्दी`, `中文`   |

## 🕒 3. Date & Time Data Types
| Data Type   | Description                                | Example               |
| ----------- | ------------------------------------------ | --------------------- |
| `DATE`      | Stores only date                           | `2025-06-26`          |
| `TIME`      | Stores only time                           | `14:30:00`            |
| `DATETIME`  | Date and time                              | `2025-06-26 14:30:00` |
| `TIMESTAMP` | Same as `DATETIME`, but often auto-updated | `CURRENT_TIMESTAMP`   |
| `YEAR`      | Year only                                  | `2025`                |

## 🔘 4. Boolean Type
| Data Type                                        | Description              | Example |
| ------------------------------------------------ | ------------------------ | ------- |
| `BOOLEAN` / `BOOL`                               | Stores `TRUE` or `FALSE` | `TRUE`  |
| (MySQL uses `TINYINT(1)` internally for BOOLEAN) | `1` or `0`               |         |



## 💾 5. Binary / Blob Data Types
| Data Type      | Description                               | Example                  |
| -------------- | ----------------------------------------- | ------------------------ |
| `BINARY(n)`    | Fixed-length binary data                  | Raw bytes                |
| `VARBINARY(n)` | Variable-length binary data               |                          |
| `BLOB`         | Binary Large Object (e.g., images, files) | Up to GBs of binary data |
| `LONGBLOB`     | Very large binary objects                 |                          |


## 🧩 6. Other Useful Data Types
| Data Type                   | Description                     | Example                       |
| --------------------------- | ------------------------------- | ----------------------------- |
| `ENUM('A', 'B', 'C')`       | List of allowed values          | `'A'`, `'B'`                  |
| `SET('X', 'Y', 'Z')`        | Multiple allowed values (MySQL) | `'X,Y'`                       |
| `UUID` / `UNIQUEIDENTIFIER` | Universally Unique Identifier   | `550e8400-e29b-41d4-a716-...` |


## 🧠 Summary Table (Quick Look)
| Category    | Common Types                            |
| ----------- | --------------------------------------- |
| Numeric     | `INT`, `DECIMAL`, `FLOAT`, `BIGINT`     |
| Character   | `CHAR`, `VARCHAR`, `TEXT`, `NVARCHAR`   |
| Date & Time | `DATE`, `TIME`, `DATETIME`, `TIMESTAMP` |
| Boolean     | `BOOLEAN`, `TINYINT(1)` (MySQL)         |
| Binary      | `BLOB`, `VARBINARY`, `LONGBLOB`         |
| Special     | `ENUM`, `SET`, `UUID`                   |




