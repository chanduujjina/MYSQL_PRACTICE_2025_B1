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
