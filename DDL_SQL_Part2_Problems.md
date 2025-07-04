## ❓ Problem 1: Insert NULL where it's not allowed
```sql
INSERT INTO students (id, name) VALUES (1, NULL);
```

### How do we prevent empty values? →  NOT NULL constraint.
## ❓ Problem 2: Insert Duplicate Records
```sql
INSERT INTO students (id, name) VALUES (1, 'Alice');
INSERT INTO students (id, name) VALUES (1, 'Bob'); -- duplicate ID
```
### How do we prevent duplicates? → Use PRIMARY KEY and UNIQUE constraints.

## ❓ Problem 3: Manually entering unique IDs every time
```sql
INSERT INTO students (id, name) VALUES (1, 'Alice');
```
-- Next time you have to figure out the next ID yourself!



