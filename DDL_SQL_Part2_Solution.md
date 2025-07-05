## ✅ Generic Syntax: CREATE TABLE with Constraints
```sql
CREATE TABLE table_name (
    column1 data_type [CONSTRAINT_NAME] constraint_type,
    column2 data_type [CONSTRAINT_NAME] constraint_type,
    ...
    [CONSTRAINT constraint_name] PRIMARY KEY (column_name),
    [CONSTRAINT constraint_name] FOREIGN KEY (column_name) REFERENCES other_table(other_column),
    [CONSTRAINT constraint_name] UNIQUE (column_name),
    [CONSTRAINT constraint_name] CHECK (condition)
);
```
## 🔑 Constraint Types in the Syntax
| Constraint    | Usage Example                              | Purpose                          |
| ------------- | ------------------------------------------ | -------------------------------- |
| `NOT NULL`    | `name VARCHAR(100) NOT NULL`               | Field cannot be null             |
| `UNIQUE`      | `email VARCHAR(100) UNIQUE`                | No duplicates allowed            |
| `PRIMARY KEY` | `emp_id INT PRIMARY KEY` or as table-level | Uniquely identifies each record  |
| `FOREIGN KEY` | `FOREIGN KEY (dept_id) REFERENCES ...`     | Enforces relationship            |
| `CHECK`       | `CHECK (age >= 18)`                        | Enforces logical condition       |
| `DEFAULT`     | `salary DECIMAL DEFAULT 30000.00`          | Default value when none provided |

## 🎯 SQL Constraints Categorized

### 🔹 1. Value-Level Constraints (Applied to Individual Columns)
   - These constraints control what kind of values can be stored in a column.

| Constraint | Meaning                               | Example                               |
| ---------- | ------------------------------------- | ------------------------------------- |
| `NOT NULL` | Value **must be provided**            | `name VARCHAR(100) NOT NULL`          |
| `DEFAULT`  | Set a **default value** if none given | `status VARCHAR(10) DEFAULT 'active'` |
| `CHECK`    | Must satisfy a **condition**          | `age INT CHECK (age >= 18)`           |
| `UNIQUE`   | Value **must be unique**              | `email VARCHAR(100) UNIQUE`           |


### 🔹 2. Key Constraints (Ensure Uniqueness and Relationships)
- These are used to identify rows uniquely and relate tables.
  
| Constraint    | Purpose                                     | Example                                            |
| ------------- | ------------------------------------------- | -------------------------------------------------- |
| `PRIMARY KEY` | Uniquely identifies each row                | `id INT PRIMARY KEY`                               |
| `FOREIGN KEY` | Links one table to another                  | `FOREIGN KEY (dept_id) REFERENCES departments(id)` |
| `UNIQUE`      | Ensures all values in a column are distinct | `UNIQUE (email)`                                   |

### 🧠 Summary Table

| Type                  | Constraint    | Use Case Example          |
| --------------------- | ------------- | ------------------------- |
| Value-Level           | `NOT NULL`    | Prevent empty name        |
|                       | `DEFAULT`     | Default status = 'active' |
|                       | `CHECK`       | Age must be > 18          |
| Identity & Uniqueness | `PRIMARY KEY` | Unique ID for each row    |
|                       | `UNIQUE`      | No duplicate emails       |
| Relationships         | `FOREIGN KEY` | Link to department table  |

### ✅ 2. Add UNIQUE to an Existing Table
- 🔸 For a single column:
```sql
 ALTER TABLE {tableName} ADD CONSTRAINT {contraint_name} UNIQUE ({columnName});
```

- 🔸 For multiple columns:
  ```sql
   ALTER TABLE {tableName} ADD CONSTRAINT {contraint_name} UNIQUE ({columnName1},{columnName2});
  ```
### ✅ 3.Add DEFAULT to Existing Column
```sql
ALTER TABLE table_name MODIFY column_name datatype DEFAULT default_value;

```

### ✅ 4.Syntax to Add CHECK Constraint to an Existing Table
```sql

ALTER TABLE table_name
ADD CONSTRAINT constraint_name CHECK (condition);
```
